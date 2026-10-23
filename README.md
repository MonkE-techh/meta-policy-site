# Monk-E Creator Intelligence — Privacy Policy Site

A dependency-free static website for the Meta app's public Privacy Policy, Terms of Service and Data Deletion Instructions URLs. The FastAPI/React application does **not** need to be hosted for these pages to be published.

## Before publishing

- Confirm Monk-E is happy to publish this policy and that it reflects the application's actual data flows, storage, providers, retention and deletion process.
- Keep `tech@monk-e.in` only if the team monitors that inbox and can action requests.
- Update the effective date and any wording that does not accurately reflect the deployed app.
- Never commit Meta app secrets, access tokens, database credentials or `.env` files to this repository.

## Publish with GitHub Pages (free for a public repository)

1. Create a **separate public repository** on GitHub, e.g. `monke-creator-intelligence-policy`. Do not publish the private application source or secrets in this repository.
2. Put `index.html`, `terms-of-service.html`, `data-deletion.html`, and this README at the repository root.
3. From PowerShell, in this folder, run (replace the URL with the repository URL you actually created):

   ```powershell
   git init
   git add index.html terms-of-service.html data-deletion.html README.md
   git commit -m "Add privacy policy and data deletion pages"
   git branch -M main
   git remote add origin https://github.com/YOUR-ORG-OR-USERNAME/YOUR-REPOSITORY.git
   git push -u origin main
   ```

4. In GitHub, open the repository's **Settings → Pages**. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/(root)`, then save.
5. Wait for GitHub Pages to publish, and copy the exact HTTPS URL shown on the Pages settings screen. Do not guess the URL.
6. Open both URLs in a private/incognito window on a device not signed into GitHub:
   - `https://YOUR-PUBLISHED-PAGES-URL/`
   - `https://YOUR-PUBLISHED-PAGES-URL/data-deletion.html`
7. Verify both pages load without a login, are readable on mobile, and that the email link opens a message to `tech@monk-e.in`.

For a project site, the deletion page is usually at `<published-base-url>/data-deletion.html`. Use the **actual** published URLs in Meta settings.

## Enter in Meta Developer Dashboard

- **Privacy Policy URL:** the public HTTPS URL of `index.html` (the published site root).
- **Terms of Service URL:** the public HTTPS URL ending in `/terms-of-service.html`. The page must contain actual service terms, not only a link to the privacy policy.
- **Data Deletion Instructions URL:** the public HTTPS URL ending in `/data-deletion.html`, if this field is available.
- If Meta specifically asks for a **Data Deletion Callback URL**, do not use this static page as the callback. A callback must be an implemented HTTPS backend endpoint that accepts Meta's signed deletion request, performs the requested deletion, and returns the response format Meta documents.

## Category

For an internal creator discovery and influencer campaign tool used by a business, **Business and pages** is the best match among the category options shown. Meta can still make independent eligibility, business verification and app-review decisions.

## Important

A public policy URL is only one submission prerequisite. It does not guarantee immediate approval or Advanced Access. Ensure the requested permissions match the actual features; complete any business verification, app review, walkthrough/screencast, deletion-flow, and data-handling requirements shown by Meta.
# meta-policy-site

## Terms of Service review

- Confirm the operating entity’s legal name, registered address and governing-law details with the organization before publishing the Terms of Service. The draft intentionally does not invent them.
- Ensure the terms accurately match the deployed application, its access model, data practices and available features.
- The terms and privacy pages are drafts for operational/product review, not legal advice and not a guarantee of Meta App Review approval.
