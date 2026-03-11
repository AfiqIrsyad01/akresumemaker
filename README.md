# AKafiq Resume Engine 🚀

> **A high-end Interactive Resume Builder SPA engineered for the Malaysian job market.**  
> Build, preview, and export professional resumes in seconds — no backend, no account, no data leaves your device.

<br>

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chartdotjs&logoColor=white)
![jsPDF](https://img.shields.io/badge/jsPDF-red?style=flat-square)
![No Backend](https://img.shields.io/badge/No%20Backend-✓-10b981?style=flat-square)
![LocalStorage](https://img.shields.io/badge/Auto--Save-LocalStorage-10b981?style=flat-square)

---

## 📸 Preview

| Creative / Modern | Minimalist | ATS-Friendly |
|:-:|:-:|:-:|
| Dark sidebar · Radar Chart · Passport photo | Clean typography · Skill bars | Plain text · Machine-readable |

---

## ✨ Features

### 🎨 Three Resume Templates

| Template | Best For | Key Characteristics |
|---|---|---|
| **Creative / Modern** | Design, Tech, ISM roles | Sidebar layout, passport photo, Radar Chart, emerald glassmorphism accents |
| **Minimalist** | Finance, Law, Management | Playfair Display typography, generous whitespace, subtle skill bars |
| **ATS-Friendly** | All corporate/government jobs | Arial font, single-column, zero images, fully machine-readable |

### 🧠 Smart Logic Guard
When **ATS Mode** is selected, the system automatically:
- Hides the passport photo
- Removes all Chart.js visualisations
- Switches to a plain single-column layout
- Ensures 100% machine-readability for Applicant Tracking Systems

### ⚡ Real-Time Live Preview
Split-panel layout — the resume preview updates **as you type**, with zero delay.

### 📊 Radar Chart (Spider Chart)
Your Technical Skills automatically populate a **Radar / Spider Chart** via Chart.js, visualising multi-domain expertise at a glance — perfect for ISM, IT, and engineering profiles.

### 💾 Auto-Save with LocalStorage
Progress is auto-saved to your browser's LocalStorage every 30 seconds. Return anytime without losing data.

### ⬇ PDF Export
One-click PDF generation using `html2canvas` + `jsPDF` — multi-page aware, maintains full styling and colours.

---

## 📋 Form Modules

### 👤 Personal Information
- Passport photo upload with live circular preview
- Name, Job Role, Phone, Email, Address, LinkedIn / Portfolio URL
- Professional Summary textarea

### 🎓 Education (Dynamic)
Add unlimited education entries. Each card includes:
- Qualification dropdown: `SPM | STPM | Sijil | Diploma | Matriks | Asasi | Degree | Master | PhD`
- Institution name, Field of Study, CGPA / Grade
- Duration / Year, Status: `Ongoing` or `Graduated`

### 💼 Work Experience (Dynamic)
Add unlimited experience entries:
- Job Title, Company, Duration, Location
- Rich freetext area for responsibilities & achievements

### 🏆 University Activities & Achievements (Dynamic)
- Activity / Role, Organisation
- Year and description

### ⚡ Skills Matrix (Three Categories)
| Category | Visualisation |
|---|---|
| Technical Skills | Sidebar progress bars + Radar Chart |
| Soft Skills | Tag pills in main body |
| Tools & Technologies | Tag pills in main body |

Each skill uses a **0–100% range slider** with live percentage display.

### ✅ Extra Benefits (Malaysian-Specific)
| Field | Options |
|---|---|
| Driver's License | D (Car) · DA (Auto) · B2 (Motorcycle) · GDL (Truck) |
| Languages | Bahasa Malaysia · English · 华语 (Mandarin) · Tamil · Arabic |
| Notice Period | Immediately Available · 1 Week · 2 Weeks · 1 Month · 2 Months · 3 Months |
| Expected Salary | Free text (e.g. RM 3,500/month) |
| Own Transport | Yes / No toggle |

### 📋 References (Dynamic)
- Full Name, Position, Company / Institution, Contact Number

---

## 🚀 Getting Started

### Option 1 — Open directly in browser (Recommended)
```
1. Download resume-builder.html
2. Double-click to open in any modern browser
3. Start filling in your details
```
No installation. No server. No dependencies to install.

### Option 2 — Serve locally (optional)
```bash
# Python
python -m http.server 8080

# Node.js
npx serve .
```
Then open `http://localhost:8080/resume-builder.html`

### Requirements
- Any modern browser (Chrome, Firefox, Edge, Safari)
- Internet connection on first load (for Google Fonts + CDN libraries)
- JavaScript must be enabled

---

## 📦 Tech Stack

| Library | Version | Purpose |
|---|---|---|
| [Chart.js](https://www.chartjs.org/) | 4.4.1 | Radar Chart / Spider Chart for skills |
| [html2canvas](https://html2canvas.hertzen.com/) | 1.4.1 | Renders the resume canvas to image |
| [jsPDF](https://github.com/parallax/jsPDF) | 2.5.1 | Converts image to downloadable PDF |
| [Google Fonts](https://fonts.google.com/) | — | DM Sans, Playfair Display, JetBrains Mono |

All libraries are loaded via CDN — no `npm install` required.

---

## 🗂 Project Structure

```
resume-builder.html     ← Single self-contained file (SPA)
README.md               ← This file
```

The entire application lives in **one HTML file** — HTML structure, Tailwind-inspired CSS, and vanilla JavaScript all included. This makes it trivially easy to host, share, or email.

---

## 💡 Usage Tips

**For the best Creative template result:**
- Upload a professional passport-style photo (square crop, JPG/PNG)
- Add at least 4–6 Technical Skills — the Radar Chart looks best with 5–8 data points
- Keep the Professional Summary to 2–3 concise sentences

**For ATS submissions:**
- Switch to ATS-Friendly mode before exporting
- Avoid special characters in job titles and company names
- Use action verbs at the start of experience bullet points (e.g. *Developed, Led, Managed*)

**For saving progress:**
- Click 💾 **Save** manually, or wait for the 30-second auto-save
- Your data persists across browser sessions via LocalStorage
- Use 🗑️ **Clear** to reset everything and start fresh

---

## 🔒 Privacy

All data is processed **entirely in your browser**.

- ✅ No data is sent to any server
- ✅ Your passport photo never leaves your device
- ✅ LocalStorage saves only to your own machine
- ✅ No account, no signup, no tracking

---

## 🛠 Customisation

To personalise the branding or colours, open `resume-builder.html` in any text editor and modify the CSS variables at the top:

```css
:root {
  --emerald-500: #10b981;   /* Primary accent colour */
  --slate-900:   #0f172a;   /* Dark background */
  --slate-800:   #1e293b;   /* Panel background */
}
```

To change the footer branding, search for `AKafiq` and replace with your own name.

---

## 🐛 Known Limitations

- PDF export of very long resumes (3+ pages) may have minor page-break alignment differences across browsers
- Passport photo crop is not built-in — crop your photo to a square before uploading for best results
- LocalStorage has a ~5MB browser limit; base64 photos consume the most space
- Internet connection required on first load for CDN fonts and libraries

---

## 🗺 Roadmap

- [ ] Drag-and-drop section reordering
- [ ] Built-in passport photo cropper
- [ ] Export as DOCX (Word format)
- [ ] Custom colour theme picker
- [ ] QR code generator for LinkedIn / portfolio
- [ ] Bahasa Malaysia / English language toggle for UI

---

## 📄 License

```
Copyright Reserved by AKafiq
All rights reserved.

This project is for personal and portfolio use only.
Redistribution or commercial use requires written permission from AKafiq.
```

---

<div align="center">

**Engineered with 💚 by AKafiq**  
*Copyright Reserved by AKafiq*

</div>
