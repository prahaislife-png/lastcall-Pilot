# LastCall Website + Legal Pages

Static website package prepared for direct GitHub/Vercel deployment.

## Deploy

1. Upload every file in this folder to the root of the Git repository.
2. Commit and push.
3. Vercel will serve the site as a static deployment. No build command is required.

## Pages

- `/` — Landing page
- `/customer-privacy` — Customer Privacy Policy (source: `4.docx`)
- `/customer-terms` — Customer Terms & Conditions (source: `5.docx`)
- `/account-deletion` — Account deletion instructions (source: `3.docx`)
- `/restaurant-privacy` — Restaurant Partner Privacy Policy (source: `1.docx`)
- `/restaurant-terms` — Restaurant Partner Terms & Conditions (source: `2.docx`)

Aliases are configured in `vercel.json` for `/privacy`, `/terms`, `/delete-account`, `/customer-account-deletion`, and `/restaurant-account-deletion`.

## Important source note

The labels written in the email do not match the actual contents of the numbered Word files. This package maps each page according to the text inside the Word documents so customer legal text is not published as restaurant legal text, or vice versa. The account-deletion page preserves `3.docx` exactly, which identifies the app as the **LastCall Restaurant Application**.

## Validation

Each Word paragraph, heading, list item, and table row was matched against its generated HTML page. The package also checks internal links, required page titles, responsive viewport tags, and `vercel.json` syntax.
