# Lens

Related: [[Photography]], [[Camera]].

- ["What is Focal Length?" - The science behind it explained. [video]](https://www.youtube.com/watch?v=xLYFEMzLtGg)
- [Angles of view and Points of view](https://www.mirrorlessons.com/2016/01/08/angle-of-view-photography/)
- https://www.reddit.com/r/photography/comments/b9g4i/comment/c0lmn30/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button

---

- Prime/zoom
- Spherical/anamorphic
- Manual/automatic

---

- Image circle
- Thread size
- Adaptors
- Stabilazation
- Telecompresor (speedbooster)/teleconverter
- [Tilt–shift photography - Wikipedia](https://en.wikipedia.org/wiki/Tilt-shift_photography)

## Focal length

Distance from point of convergence to sensor.

Wide (18mm) to narrow (55mm)

[Angle of view (photography) - Wikipedia](https://en.wikipedia.org/wiki/Angle_of_view_(photography))

```typescript
const angle_of_view = Math.atan2(Math.sqrt(36 ** 2 + 24 ** 2) / 2, 50) * 2 *
	180 / Math.PI;
```

## Aperture

```typescript
const focal_length = 50; // mm
const f_number = 2.8;
const aperture = focal_length / f_number;
```

### f-number

[f-number - Wikipedia](https://en.wikipedia.org/wiki/F-number)

Smaller number is wider (maximum, fast) and larger number is narrower/telephoto (minimum, slow).

```typescript
const focal_length = 50; // mm
const aperture = 10; // mm
const f_number = focal_length / aperture;
```

Meaning that the maximum and minimum aperture change with the focal length.

## Autofocus motor

- DC: Old, cheapest
- STM: Quiet AF, smooth, cheaper
- USM: Louder AF, fast, manual

## Canon

- [Canon lens compatibility](https://www.eos-magazine.com/articles/eospedia/canon-lens-compatibility.html)
- [Compatibility Guide for Lenses - Canon Ireland](https://www.canon.ie/lenses/compatibility/)

| Mount                                                               | Native compatability | Adaptor compatability | Size       | Release date | Notes             |
| ------------------------------------------------------------------- | -------------------- | --------------------- | ---------- | ------------ | ----------------- |
| [EF](https://en.wikipedia.org/wiki/Canon_EF_lens_mount), TS-E, MP-E | EOS DSLRs and SLRs   | EOS-EF M, EOS-EF R    | Full-frame | 1987 (EF)    | Tilt shift, macro |
| [EF-S](https://en.wikipedia.org/wiki/Canon_EF-S_lens_mount)         | APS-C EOS DSLRs      | EOS-EF M, EOS-EF R    | APS-C      | 2003         |                   |
| [EF-M](https://en.wikipedia.org/wiki/Canon_EF-M_lens_mount)         | EOS-M                | None                  | APS-C      | 2012         | Cropped           |
| [RF](https://en.wikipedia.org/wiki/Canon_RF_lens_mount)             | EOS-R                | None                  | Full-frame | 2018         |                   |
| [RF-S](https://en.wikipedia.org/wiki/Canon_RF_lens_mount)           | EOS-R                | None                  | APS-C      | 2022         |                   |

## Brands

Other than by camera manufacturer.

- Carl Zeiss
- Olympus
- Tamron
- Panasonic
- Sigma
- TTArtisan
- 7Atrisans
