# Tagged union

```typescript
class Paragraph {
  readonly type = "Paragraph";
  constructor(public content: string) {}
}

class BlankLine {
  readonly type = "BlankLine";
}

type Block = Paragraph | BlankLine;

const block = new Paragraph("Hello, world!") as Block;

switch (block.type) {
  case "Paragraph": {
    console.log("Paragraph");
    break;
  }

  case "BlankLine": {
    console.log("Blank line");
    break;
  }

  default: {
    block satisfies never;
  }
}
```

```rust
enum Block {
	Paragraph(String)
	EmptyLine
}

let block = Block::Paragraph("Hello, world!");

match block {
	Block::Paragraph => println!("Paragraph")
	Block::EmptyLine => println!("Empty line")
}
```
