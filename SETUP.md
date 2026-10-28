# Setup checklist (for the author; delete this file before going public)

1. Fill the placeholders: OWNER/REPO (docs/index.html, README.md), WORKBOOK-ADDRESS (README.md, LICENSE.md, docs/index.html), INSTRUCTOR-CONTACT (README.md, docs/index.html), YEAR (LICENSE.md), DATE (CHANGELOG.md).
2. Put each chapter's starting workbooks in workbooks/chNN/. File names should match the names the book prints with \workbook{...}, plus .xlsx. No solution workbooks.
3. Check each workbook for hidden sheets, personal information (File > Info > Inspect Workbook), and leftover answers in cells the labs ask readers to fill.
4. Create a public repository on GitHub and push these files. Keep the repository private until steps 1 to 3 are done.
5. Settings > Pages: Source "Deploy from a branch", branch main, folder /docs.
6. Custom address: rename docs/CNAME.example to docs/CNAME with your address in it, add the DNS record GitHub Pages asks for at your domain registrar, and turn on Enforce HTTPS.
7. Release: git tag v1.0 and git push origin v1.0. The workflow in .github/workflows/release.yml builds the zips and attaches them to the release. Then click every download link on the page once.
8. Book: replace the copyright-page placeholder with the address, and add "Workbook version 1.0 matches this printing."
