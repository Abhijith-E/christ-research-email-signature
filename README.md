# CHRIST University Email Signature Pack
**"Quiet Prestige" Design Edition**

This package contains a production-ready, institution-grade email signature tailored for a Research Assistant at the Centre for Quantum Technologies and Complex Systems (CQTCS), CHRIST (Deemed to be University).

## Design Rationale
The design adheres to the "Quiet Prestige" aesthetic used by faculty at top-tier research institutions (MIT, Stanford, Oxford). 
- **Typography as Hierarchy:** The name is set in a robust Serif font (Georgia) to anchor the design, while the titles and details are in a clean, legible Sans-serif (Arial). 
- **Restrained Color:** A strict grayscale palette combined with the official CHRIST University Blue (`#2957A4`) used only for the vertical accent divider and links. No bright social media icons or distractive graphics.
- **Minimalist Architecture:** The layout relies on strict vertical alignment and generous whitespace rather than borders or background colors. 
- **Understated Links:** Social/portfolio links are rendered as muted text labels. This ensures zero rendering issues across email clients (which often butcher complex multi-color SVG/PNG icon grids) and maintains the serious, academic tone.

## Included Files
- `index.html` - The primary signature file, optimized for modern clients (Gmail, Apple Mail).
- `outlook.html` - A flat-table variant explicitly hardened for Outlook Desktop.
- `signature.txt` - A clean plain-text fallback.
- `signature.docx` - A Word document version for pasting into the Outlook signature editor.
- `preview.png` - A visual reference of the final rendered signature.
- `christ-logo-transparant.png` - A scaled placeholder logo. 

---

## Pre-Installation Steps

1. **Fill in Placeholders:** Open `index.html` (and/or `outlook.html`) in a basic text editor (like VS Code, Notepad, or TextEdit) and replace `[[FILL ME: Official Email]]` with your actual email address.
2. **Host the Logo Image:** 
   Email clients *cannot* embed local images directly from your computer. You must upload `christ-logo-transparant.png` (or your final CHRIST University logo) to a public server. 
   - **Recommended:** Upload it to an AWS S3 bucket, a personal domain, or use a reliable image hosting service (like Imgur). 
   - **Alternative:** You can upload it to GitHub and use the *Raw* URL (e.g., `https://raw.githubusercontent.com/.../christ-logo-transparant.png`).
   - Once uploaded, replace `https://example.com/christ-logo-transparant.png` in the HTML files with your actual public URL.

---

## Installation Guide

### Gmail (Web)
1. Open `index.html` in your web browser (Chrome, Safari, Firefox).
2. Select everything on the page (`Ctrl + A` or `Cmd + A`) and Copy (`Ctrl + C` or `Cmd + C`).
3. Open Gmail and go to **Settings** (the gear icon) > **See all settings**.
4. Scroll down to the **Signature** section.
5. Create a new signature (or edit an existing one).
6. Click into the signature text box and Paste (`Ctrl + V` or `Cmd + V`).
7. Scroll to the bottom and click **Save Changes**.

### Apple Mail (macOS)
1. Open `index.html` in Safari or Chrome.
2. Select all (`Cmd + A`) and Copy (`Cmd + C`).
3. Open Apple Mail and go to **Mail > Settings** (or Preferences) > **Signatures**.
4. Select your email account in the left column.
5. Click the `+` button to add a new signature.
6. Uncheck "Always match my default message font".
7. Paste (`Cmd + V`) the signature into the right-hand box. (Note: The images might appear as blank boxes in the preview window, but they will render correctly when you compose an email).

### Outlook Desktop (Windows)
1. Open the provided `signature.docx` file in Microsoft Word.
2. Select the entire table (`Ctrl + A` or click the table selector handle in the top-left corner).
3. Copy the selection (`Ctrl + C`).
4. Open Outlook and go to **File > Options > Mail > Signatures**.
5. Create a new signature.
6. Paste the copied content into the signature editor box (`Ctrl + V`).
7. Click **OK** to save.
*(If you experience any spacing issues, you can alternatively try copying directly from the `outlook.html` file opened in a web browser).*

### Outlook (Web / Office 365)
1. Open `index.html` in your browser.
2. Select all (`Ctrl + A` or `Cmd + A`) and Copy.
3. Go to Outlook Web, click the **Settings** gear icon.
4. Go to **Mail > Compose and reply**.
5. Paste the signature into the editor box.
6. Click **Save**.

---

## Future Updates
To update your titles or links, you can edit the HTML file in a text editor and repeat the installation process. Be careful not to delete any `<td>` or `<tr>` tags, as this will break the table layout.
