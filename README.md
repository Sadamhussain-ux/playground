# Breakpoint Bench

See any website at four screen sizes side by side, in one view.

| Frame            | Breakpoint | Default size |
|------------------|------------|--------------|
| Mobile           | < 500px    | 390 × 780    |
| Tablet portrait  | > 520px    | 600 × 880    |
| Tablet landscape | > 760px    | 880 × 620    |
| Desktop          | > 992px    | 1366 × 768   |

Each frame's width and height can be edited under the frame. "Fit to window" scales all four together so they fit on one screen; untick it to see them at 100%.

## Use

Type a URL and press **Load**. You can also share a direct link:

```
https://<your-username>.github.io/<repo-name>/?url=https://example.com
```

## Deploy on GitHub Pages

1. Create a new repository on GitHub and upload `index.html` (and this README).
2. Go to **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then **Save**.
4. After a minute the site is live at `https://<your-username>.github.io/<repo-name>/`.

## If a frame stays blank

Some sites send `X-Frame-Options: DENY/SAMEORIGIN` or a `Content-Security-Policy: frame-ancestors` header, which stops browsers from showing them inside another page. Large sites (Google, Facebook, banks) usually do this. For your own site, allow framing from your GitHub Pages domain, or run this viewer on `localhost` while you develop.
