# TigerPaw website

Static HTML/CSS site: homepage, seven service pages and a 404 page.

## Before you deploy
1. Create a free form at https://formspree.io (sign up with the email that should receive enquiries).
2. Copy your form ID (it looks like `xayzabcd`).
3. In `index.html`, replace `YOUR_FORM_ID` in the form's `action` with your ID.

## Deploy to AWS Amplify (no Git needed)
1. AWS Console > Amplify > Create new app > Deploy without Git.
2. Upload `tigerpaw-site.zip` (files must sit at the root of the zip, which they do).
3. Open the temporary amplifyapp.com address and check every page and the contact form.
4. App settings > Custom domains > Add domain > tigerpaw.com.au. Amplify creates the Route 53 records and SSL certificate.
5. To update the site later, edit the files, re-zip them and upload a new deployment.

## Editing
- Text is in the `.html` files. Colours and fonts are in `styles.css` (see the `:root` variables at the top).
