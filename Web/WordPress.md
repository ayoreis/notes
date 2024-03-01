# Wordpress

## Setup

[Wordpress - ArchWiki](https://wiki.archlinux.org/title/Wordpress)

- Download from [WordPress.org](https://wordpress.org) or direcly from server for more reproducibility.
- The WordPress and site addresses need to be lowercase or else WordPress will enter a redirection loop (type `Maze.local` -> browser will lowercase it into `maze.local` -> Worpress will redirect back to `Maze.local`, loop).
- WordPress importer never worked for me, instead download the `uploads` directory and export/import the database in phpMyAdmin.
- Enable `define( 'WP_DEBUG', true );` in `wp_config.php`.
