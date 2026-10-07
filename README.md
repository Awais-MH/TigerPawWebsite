# TigerPaw website

Static HTML/CSS site: homepage, seven service pages and a 404 page.

## Before you deploy
The "Book a free chat" form in `index.html` sends enquiries to info@tigerpaw.com.au via https://formsubmit.co (free, no account).
1. After deploying, submit the form once yourself. FormSubmit emails info@tigerpaw.com.au an activation link; click it. Enquiries are only delivered after activation.
2. Optional: the activation email includes a random alias. Replace `info@tigerpaw.com.au` in the form's `action` with that alias to keep the address out of the page source.
3. To change the receiving address, edit the form's `action` URL (and re-activate).

## Deploy to AWS Amplify (no Git needed)
1. AWS Console > Amplify > Create new app > Deploy without Git.
2. Upload `tigerpaw-site.zip` (files must sit at the root of the zip, which they do).
3. Open the temporary amplifyapp.com address and check every page and the contact form.
4. App settings > Custom domains > Add domain > tigerpaw.com.au. Amplify creates the Route 53 records and SSL certificate.
5. To update the site later, edit the files, re-zip them and upload a new deployment.

## Editing
- Text is in the `.html` files. Colours and fonts are in `styles.css` (see the `:root` variables at the top).
