# X Publishing Manager — public information website

This directory contains only the public static information website. It is
separate from the private FastAPI application in ../X.

Publish only these files to a dedicated public repository:

- index.html
- .nojekyll
- README.md

Configure GitHub Pages to deploy from the main branch, root directory. Use the
actual URL returned by GitHub Pages, verify its HTTPS response and rendered page,
then use that exact address as X Developer Console's Website URL.

No custom domain, external assets, scripts, build tools, or application secrets
are required. Do not copy the parent workspace or private application into this
repository. The local OAuth callback stays
http://localhost:8000/auth/x/callback and does not point to this static site.
