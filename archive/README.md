# WordPress archive

Raw archive of the old site **sebneumaier.wordpress.com**, kept so nothing is lost
after WordPress is shut down. Not linked from the live site.

- `wordpress-posts.json` / `wordpress-pages.json` — full content dump of all posts
  and pages (WordPress.com REST API, `content.rendered`).
- `posts/` — each post and page rendered as a standalone, readable HTML file.
  Upload links inside were rewritten to the local copies under `../files/`.

The uploaded documents themselves (PDFs, slides, …) live in `/files`, mirroring the
original `wp-content/uploads/YYYY/MM/` structure. A browsable overview is at
[`/documents.html`](../documents.html).
