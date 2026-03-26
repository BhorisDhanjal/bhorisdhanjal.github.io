# bhorisdhanjal.github.io

My professional academic website (Jekyll + custom theme for PhD portfolio).

**See `DEVELOPMENT.md` (local file) for detailed personal instructions on adding blog posts, folder structure, review steps, and long-term maintenance.**

## Features
- Clean academic design with projects and blog
- MathJax for equations, syntax highlighting for code
- Tag-based blog with search and RSS feeds
- Responsive, mobile-friendly layout

## Quick Setup
1. Install Ruby + Bundler (`sudo apt install ruby-full` or similar on Linux).
2. `bundle install`
3. `bundle exec jekyll serve` → preview at http://localhost:4000
4. Make changes, test, then `git push` to `main` (GitHub Pages auto-deploys).

## Folder Structure (Key Directories)
- `_posts/`: Add new blog posts here (see DEVELOPMENT.md for template).
- `_projects/`: Markdown files for project pages.
- `_pages/`: Static pages (blog.md, cv.md, projects.md).
- `_layouts/`, `_includes/`: Templates and reusable HTML.
- `assets/`: Images, PDFs, CSS (copied to `_site/` on build).
- `_config.yml`: Site config, permalinks, plugins.
- `_site/`: Generated output (ignored by git).

## Review Steps Before Pushing (Summary)
1. `git status` / `git diff`
2. `bundle exec jekyll build` (fix any errors)
3. `bundle exec jekyll serve` and manually test:
   - Blog page, individual posts, math rendering
   - Search, tags, links, mobile view
4. Check generated files in `_site/`
5. Commit with clear message and push to `main`

For full details + how to post new content yourself, see `DEVELOPMENT.md`.

See `_config.yml` for more settings. The site uses a custom `_plugins/tags.rb` for auto tag pages.
