# Zoomlit Studio

Static site, no build step.

- `index.html`: landing page (features, how it works, About us, Contact us)
- `app.html`: the editor
- `assets/`: demo clips, video posters, share image (`og-image.png`) and icons (`icons/`)
- `favicon.ico`, `manifest.webmanifest`: site icon and web app manifest
- `robots.txt`, `sitemap.xml`: SEO files

## Before you publish

1. **Domain:** replace `https://your-domain.com` with your real URL in `index.html`, `app.html`, `robots.txt` and `sitemap.xml`.
   Example: `sed -i 's#https://your-domain.com#https://zoomlit.vercel.app#g' index.html app.html robots.txt sitemap.xml`
2. **Contact email:** set to salemaymen814@gmail.com via `CONTACT_EMAIL` near the bottom of `index.html`.
   The contact form posts directly through FormSubmit. The first message you send triggers an activation email; click the link once and the form is live.

Deploy: drag the folder into Vercel or Netlify, or run `npx serve .` locally.
After deploying, submit `sitemap.xml` in Google Search Console.
