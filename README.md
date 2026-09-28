# Modern Developer & Designer Portfolio

A sleek, responsive, and high-performance personal portfolio website built with modern HTML5, Tailwind CSS, custom glassmorphism styling, and interactive JavaScript.

---

## 🚀 Quick Start

### 1. View in Browser
Simply double-click [`index.html`](./index.html) or run a quick local development server:

```bash
# Using Python 3:
python -m http.server 3000

# Using Node.js (npx):
npx serve
```
Then visit `http://localhost:3000` in your web browser.

---

## 📁 Project Structure

```text
portfolio/
├── index.html       # Main structural markup & sections (Hero, About, Skills, Projects, Contact)
├── style.css        # Custom glassmorphism, glowing orbs, scrollbar, and badge styling
├── script.js       # Typewriter animation, category filters, mobile menu, and form feedback
└── README.md        # Documentation and deployment instructions
```

---

## 🎨 Customization Guide

### 1. Personal Info & Hero Section
Open [`index.html`](./index.html) and update:
- **Name & Brand**: Search for `Alex Morgan` and `Alex.dev` to replace with your name.
- **Dynamic Typewriter Titles**: In [`script.js`](./script.js#L8-L15), edit the array `words`:
  ```javascript
  const words = [
    'Full-Stack Engineer',
    'UI/UX Craftsman',
    'Cloud Systems Architect',
    'Open Source Builder'
  ];
  ```

### 2. About & Experience
- Update the bio paragraphs and job highlights under `<section id="about">` in [`index.html`](./index.html).
- To link your resume, update the `href` attribute on the `Download Resume (PDF)` button.

### 3. Skills & Technologies
- Add or remove tags in `<section id="skills">`. Simply duplicate `<span class="skill-tag">...</span>` with your favorite technologies.

### 4. Projects Showcase
- Add your own projects in `<section id="projects">`.
- Set the `data-category` attribute on each `.project-card` (`fullstack`, `frontend`, or `ai`) to integrate with the interactive filter buttons.
- Update project titles, descriptions, live demo links, and GitHub repository links.

### 5. Contact Form & Socials
- Update your email address and social links (GitHub, LinkedIn, Twitter/X) in `<section id="contact">`.
- To connect the contact form to a real backend service, you can plug in free providers like [Formspree](https://formspree.io) or [EmailJS](https://www.emailjs.com).

---

## 🌐 Free 1-Click Deployment

### Option A: GitHub Pages
1. Push the `portfolio` folder to a GitHub repository.
2. In GitHub, go to **Settings > Pages**.
3. Under **Branch**, select `main` (or `master`) and `/root`, then click **Save**.
4. Your portfolio will be live at `https://<username>.github.io/<repo-name>/`.

### Option B: Vercel / Netlify
- Drag and drop the `portfolio` folder directly into [Vercel](https://vercel.com) or [Netlify](https://netlify.com) for instant global edge deployment with free SSL.
