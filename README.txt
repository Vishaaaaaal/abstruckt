
ABSTRUCKT — static site (Figma > code)

Files:
- index.html — single-page landing built from your “Abstruckt Home” frame
- styles.css — minimal, production-ready CSS
- assets/ — drop your images here:
  - hero-main.jpg (hero image of the model/tee)
  - nurburgring.png (track outline graphic)
  - tee-front.jpg, tee-back.jpg, wide-shot.jpg (collection images)

Deploy (GitHub Pages + custom domain abstruckt.com):
1) Create a repo named `abstruckt.com` (or any) and push these files.
2) In GitHub → Settings → Pages → Build from `main` (root).
3) Add a `CNAME` file in the repo root with one line: abstruckt.com
4) In your domain DNS (at your registrar), add:
   - A @ → 185.199.108.153
   - A @ → 185.199.109.153
   - A @ → 185.199.110.153
   - A @ → 185.199.111.153
   - (Optional) CNAME www → <your-username>.github.io
5) Wait for DNS to propagate, then test https://abstruckt.com

Notes:
- Replace placeholder images under /assets/.
- Typography and layout mirror the Figma structure, mobile responsive.
- All icons are inline SVG (no external libs).
- Tweak palette in :root variables inside styles.css.
