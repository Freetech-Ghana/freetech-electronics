# Freetech Electronics — Request a Project

New `project-request.html` provides a global business-service inquiry form. A service CTA is also inserted near the contact section of both existing storefront variants (`Freetech Electronics.html` and `man.html`). Existing product and checkout JavaScript is preserved.

Deploy `project-request.html`, `intake-config.js` and the correct updated storefront HTML in the **same directory** as the live site.

Only after a properly secured public HTTPS intake API has been deployed, update `intake-config.js`:

```js
window.FREETECH_INTAKE_URL = 'https://YOUR-INQUIRY-DOMAIN';
```

Never store private sync tokens in that file. If left empty, the form opens a visitor-controlled email draft for `danielantwi901@gmail.com` and does **not** claim server submission.

Public intake backend: `Freetech-Ghana/freetech-jarvis-ai` branch `feature/aiva-public-inquiries-20261107`.

Production requires correct DNS, HTTPS/TLS, permitted origins, rate limits and a privacy notice. No deployment has been performed by these commits.