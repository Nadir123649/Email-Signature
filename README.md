# Preston & Co. Property Buyers — Email Signatures

This repository contains the official, mobile-responsive HTML email signature templates for the **Preston & Co. Property Buyers** team. These signatures are optimized for high cross-client compatibility (Gmail, Apple Mail, Outlook, etc.) and feature a premium dark-gray and gold aesthetic.

---

## 📋 Table of Contents
1. [Team Signatures Overview](#-team-signatures-overview)
2. [Design & Technical Details](#-design--technical-details)
3. [How to Use / Installation Guide](#-how-to-use--installation-guide)
4. [Customization & Editing](#-customization--editing)
5. [Assets & Branding](#-assets--branding)

---

## 👥 Team Signatures Overview

The repository consists of three distinct signature templates:

| File | Team Member | Role | Email | Phone | Name Header Image |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **[index.html](file:///d:/Projects%20Company/Email-Signature/index.html)** | **Josh Preston** | Director & Buyers Agent | [josh@prestonandco.com.au](mailto:josh@prestonandco.com.au) | `0416 968 734` | [Josh Name Image](https://res.cloudinary.com/df80crgrw/image/upload/e_trim/v1782286792/Josh_Preston_yjovlz.png) |
| **[second.html](file:///d:/Projects%20Company/Email-Signature/second.html)** | **Sophie Preston** | Buyers Associate and Administration | [sophie@prestonandco.com.au](mailto:sophie@prestonandco.com.au) | `0458 253 836` | [Sophie Name Image](https://res.cloudinary.com/df80crgrw/image/upload/e_trim/v1782289972/Sophie_Preston_dcljgx.png) |
| **[three.html](file:///d:/Projects%20Company/Email-Signature/three.html)** | **Kiyah Preston** | Operations Manager | [kiyah@prestonandco.com.au](mailto:kiyah@prestonandco.com.au) | `0458 253 836` | [Kiyah Name Image](https://res.cloudinary.com/df80crgrw/image/upload/e_trim/v1782290025/Kiyah_Preston_cy8kln.png) |

---

## 🎨 Design & Technical Details

The signature layouts have been engineered specifically to withstand the quirks of various email clients:

- **Typography**: Uses modern sans-serif typography (`'Montserrat'`, `'Helvetica Neue'`, `Helvetica`, `Arial`, `sans-serif`) to ensure an elegant look across all platforms.
- **Palette**:
  - Primary Dark: `#353A3D` (Charcoal Gray)
  - Secondary Accent: `#DCBB9A` (Gold/Sand)
  - Background: `#F6F5F4` (Warm Light Gray)
  - Text Color: `#353A3D` / `#686C6E` (Secondary Gray)
- **Responsive Layout**:
  - **Desktop (600px width)**: Side-by-side layout with a dark logo card on the left, a gold vertical divider, and contact info + custom name script graphic on the right.
  - **Mobile (<480px width)**: Stacks vertically. The logo card goes to the top, vertical separators are hidden, and content centers/scales appropriately for small screens.
- **Client Bug Mitigation**:
  - Includes a `.gmail-fix` spacer at the bottom to prevent layout squishing or truncation in the Gmail mobile app.
  - Built entirely using tables (`<table>`, `<tr>`, `<td>`) with inline CSS styling for maximum layout preservation.

---

## 🚀 How to Use / Installation Guide

To set up your signature, follow either the **visual copy-paste method** (recommended for Gmail & Outlook) or the **direct HTML method**.

### Method 1: The Visual Copy-Paste (Easiest)
1. Open the desired signature HTML file (e.g., `index.html`) in any web browser (Double-click the file).
2. Press `Ctrl + A` (Windows) or `Cmd + A` (Mac) to select the entire page content.
3. Press `Ctrl + C` (Windows) or `Cmd + C` (Mac) to copy it.
4. Open your email client signature settings (e.g., Gmail Settings -> General -> Signature).
5. Paste (`Ctrl + V` / `Cmd + V`) the signature into the signature edit box.
6. Make sure to **save changes** at the bottom of the settings page.

### Method 2: Direct HTML Insertion (Outlook/Apple Mail)
If your email client supports editing the signature's HTML source file directly:
1. Open the HTML file in a code editor or text editor.
2. Copy the entire raw HTML code.
3. Paste it into your email client's signature HTML source folder/settings.

---

## ⚙️ Customization & Editing

If you need to update a phone number, change an email address, or update a name image, make sure to follow these guidelines:

### 1. Modifying Text Fields
Ensure you update both the **hyperlink target** and the **display text**. For example, in the phone row:
```html
<a href="tel:0416968734" style="color: #353A3D; ...">0416 968 734</a>
```
*Make sure the `href` attribute matches the display text to avoid calling the wrong number.*

### 2. Updating Script Name Images
The signature uses transparent PNG images for the handwritten/script names, hosted on Cloudinary.
- To swap a script name, upload the transparent PNG to your image host (e.g., Cloudinary) and replace the URL in the `<img>` tag:
  ```html
  <img src="YOUR_CLOUDINARY_URL_HERE" alt="Name" width="220" class="name-image" style="display: block; border: 0; width: 220px; height: auto;" />
  ```
- **Note**: The class `.name-image` handles responsive resizing on mobile screens, so preserve this class name and inline style attributes.

---

## 📂 Assets & Branding

- **Website**: [prestonandco.com.au](https://prestonandco.com.au)
- **Tagline**: `FROM COUNTRY TO THE COAST.`
- **Instagram**: [@prestonandco_propertybuyers](https://instagram.com/prestonandco_propertybuyers)
- **Servicing Region**: Sunshine Coast & Surrounds
