# georgeaw.com

An Astro static site

## Layout

- `src/pages/` contains the Home, CV, and Publications Markdown pages.
- `src/content/blog/` contains the blog posts.
- `src/pages/blog/` contains the generated archive and individual-post routes.
- `public/images/` contains the two Copycat screenshots used by the Copycat
  post. Astro exposes these as `/images/...`.

Blog routes use Astro's standard `/blog/<post-slug>/` convention.

Static page routes are created from their filenames: `/`, `/cv/`, and
`/publications/`.

## Run locally

```sh
npm install
npm run dev
```
