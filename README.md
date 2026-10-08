# trettlabs.com

The company website for Trett Labs Limited: one static page with what we do, our apps (linking to
beequation.com), contact and the company details UK law requires (name, number, place of registration,
registered office). No build step, no cookies, analytics or third-party requests (fonts are self-hosted).

## Hosting (GitHub Pages)
Settings → Pages: deploy from branch `main`, folder `/`, custom domain `trettlabs.com` (the `CNAME` file sets it).

DNS at 123-reg for trettlabs.com (Manage DNS):
- Remove the existing A records for `@` (123-reg's parking page).
- A records for `@`: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
- CNAME for `www`: `trettbob.github.io`
- Keep the Google Workspace MX/TXT records as they are.

Then tick "Enforce HTTPS" in Pages settings once it's offered.
