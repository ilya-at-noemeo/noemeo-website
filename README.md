# noemeo-website

The public one-page site at https://noemeo.com, served by GitHub Pages
from `main` (`CNAME` holds the custom domain). Plain HTML and CSS in
`index.html`, no build step.

`checkout/sandbox/` is Paddle's default payment link for the sandbox
account: a static page that loads Paddle.js so Paddle's checkout opens
for a transaction the Noemeo app started (`?_ptxn=...`). It holds a
client-side token, which is public by design; no secret ever goes on
this site. The live page (`checkout/`) comes with the live Paddle
account. See noemeo-photo's `docs/accounts-and-billing-design.md`.

Keep its claims true to the product: what Noemeo does, and especially
the privacy section, must match noemeo-photo's actual behaviour (photos
and conversations stay on the user's computer; the cloud runs model
calls and accounts only).
