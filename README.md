# Multi-Page Modern Static Website (HTML5, CSS3, JavaScript)

A gorgeous, highly professional 4-page static website built with modern CSS custom properties, glassmorphic UI components, smooth scroll animations, and a structured folder layout (`css/`, `js/`, `assets/`). Perfect for practicing static site deployments on AWS S3, CloudFront, and CI/CD static pipelines.

## 🚀 Pages Included
1. **Home (`index.html`)**: Hero banner, feature highlights, and interactive metrics counter.
2. **About (`about.html`)**: Company mission, team values, and interactive stats.
3. **Services (`services.html`)**: Interactive service cards with hover glow effects and pricing tier toggles.
4. **Contact (`contact.html`)**: Fully interactive contact form with client-side validation and success toast alert.

---

## 📂 Folder Structure
```text
aws_devops_multipage_website/
├── index.html
├── about.html
├── services.html
├── contact.html
├── css/
│   └── style.css
├── js/
│   └── main.js
└── assets/
    └── images/
```

## 🛠️ Deployment Instructions
1. Extract this zip file.
2. Open `index.html` in any browser or serve locally using `npx serve` or Live Server.
3. To deploy on AWS, upload these static files directly to an **AWS S3 bucket** configured for static website hosting, or set up an **AWS CodePipeline** with GitHub to automate deployments.
