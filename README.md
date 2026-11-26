# CYBER OPS — Unit 11 | Release 1.0

Standalone classroom practice for Pearson BTEC Level 3 Nationals in IT, Unit 11 (20158K). Original implementation informed by the public PGHUB2022 Operation Ghost Laptop site: https://pghub2022.github.io/operation-ghost-laptop/ . The source HTML was inspected via web access; the repository archive could not be retrieved into the build environment. No upstream source files, assets, credentials or Firebase configuration are included. The original website is linked as an optional extension. Check upstream permissions before incorporating any of its assets later.

## Run locally
Extract the ZIP. Open `site/index.html` in Edge or Chrome. No installation, server, accounts or external services are needed for the core modules. The optional original website link requires internet. Browser local-storage behaviour for file URLs varies; export your responses before closing. Speech support depends on browser/OS voices.

## Deploy to your GitHub account
1. Visit https://github.com/new and create a separate public repository called `btec-unit11-cyber-security` under PGHUB2022. Do not change the original Operation Ghost Laptop repository.
2. In the new repository choose Add file > Upload files (or the upload link on an empty repository). Upload **the contents of the site folder**, not the enclosing folder. Keep evidence/ and its files together. If the browser upload does not preserve folders, use GitHub Desktop or the command line below.
3. Commit to main. Open Settings > Pages. Source: Deploy from a branch; branch main; folder / (root); Save.
4. Check the Pages deployment workflow has succeeded. Visit https://pghub2022.github.io/btec-unit11-cyber-security/ (expected address, not yet deployed).
5. Test on a student computer: navigate eight modules, enter and export responses, refresh, download evidence, change font and contrast, and reset. Confirm with IT that site is permitted.

### Git alternative (PowerShell, from extracted `site` directory)
Create an empty repository first; authenticate using Git Credential Manager or GitHub CLI. Do not paste credentials into code.
```powershell
git init -b main
git add .
git commit -m "Initial CYBER OPS classroom release"
git remote add origin https://github.com/PGHUB2022/btec-unit11-cyber-security.git
git push -u origin main
```

## Important
Keep `teacher/` outside the public repository. The quiz answers are client-side and can be inspected: exam mode hides feedback but does not enforce secure conditions. This is formative practice, never a live external assessment environment. Written answers need human assessment. No central tracking, teacher login or leaderboard is implemented. Local browser storage is not secure; do not enter real personal or sensitive information. Export to the college-approved submission platform, then reset shared computers. No real malicious files, executable samples or external targets are included.

## Modify
Edit `site/content.js` for case, task, quiz and glossary content; `site/style.css` for appearance; `site/app.js` for behaviour. Quiz answer indexes are zero-based strings. Update evidence links in app.js when filenames change. Recompute the manifest after modifying evidence (PowerShell Get-FileHash -Algorithm SHA256 or sha256sum). Use a separate browser profile to test revisions. The risk scale is a teaching choice, not a mandated Pearson scale.

## Curriculum references
Pearson BTEC Nationals IT (2016), delivery guide: https://qualifications.pearson.com/content/dam/pdf/BTEC-Nationals/Information-Technology/2016/teaching-and-learning-materials/btec-delivery-guide.pdf
Pearson getting ready to teach: https://qualifications.pearson.com/content/dam/pdf/BTEC-Nationals/Information-Technology/2016/teaching-and-learning-materials/pearson-btec-level-3-national-in-information-technology-2016-and-2017-getting-ready-to-teach.pdf
Use the actual current Pearson task instructions and templates for formal practice. This package uses original fictional tasks, not official questions or grade boundaries.
