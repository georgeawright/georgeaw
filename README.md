# georgeaw.com

This is a conventional Astro static site, migrated from the public WordPress
pages and posts available on 12 October 2026.

## Layout

- `src/pages/` contains the Home, CV, and Publications Markdown pages.
- `src/content/blog/` contains the two published posts, validated by the typed
  collection in `src/content.config.ts`.
- `src/pages/blog/` contains the generated archive and individual-post routes.
- `public/images/` contains the two Copycat screenshots used by the Copycat
  post. Astro exposes these as `/images/...`.

Blog routes use Astro's standard `/blog/<post-slug>/` convention. The static
page routes are created from their filenames: `/`, `/cv/`, and
`/publications/`.

## Run locally

```sh
npm install
npm run dev
```

Use `npm run build` to create the production site in `dist/`. GitHub Pages can
deploy that directory from the included GitHub Actions workflow. The included
`public/CNAME` configures the intended custom domain, `georgeaw.com`; configure
the corresponding DNS records and select **GitHub Actions** as the Pages source
after pushing this directory as its own GitHub repository.

WordPress-only material has not been migrated: navigation markup, theme CSS,
the comments form, author byline, and generated post-navigation controls.
