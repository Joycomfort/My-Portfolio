# AI Portfolio Website

A modern, responsive portfolio website for an aspiring AI developer.
Built with plain HTML, CSS, and JavaScript — beginner-friendly and easy to customize.

## Folder Structure

```
ai-portfolio/
├── index.html          # Main page (all sections)
├── css/
│   └── styles.css      # All styles (dark/light theme)
├── js/
│   └── main.js         # Interactivity: theme, menu, particles, form validation
├── assets/
│   └── images/         # Put screenshots / project images here
└── README.md
```

## Run Locally

No build step required. Just open the file:

- **Option 1:** Double-click `index.html` to open in your browser.
- **Option 2:** Use VS Code "Live Server" extension for auto-reload.
- **Option 3:** Serve with Python:
  ```
  python -m http.server 8000
  ```
  Then visit http://localhost:8000

## Customize

Search for these placeholders in `index.html` and replace them:

- `OKONKWO JOY` — your name
- `joycomfort12@gmail.com` — your email
- `https://github.com/Joycomfort` — your GitHub URL
- `https://linkedin.com/in/okonkwo-joy` — your LinkedIn URL
- `Nigeria` — your location

### Add a project
Duplicate a `<article class="project-card">` block in the Projects section.
Change the title, purpose, problem, tech tags, and features.
When a project is done, change `status-planned` to `status-done` and update the label to "Completed".
Replace the `#` links with real source/demo URLs.

### Add an achievement
In the Achievements section, replace the placeholder with cards, e.g.:
```html
<div class="about-card">
  <h3>Certificate Name</h3>
  <p>Issuer — Year</p>
</div>
```

### Contact form backend (optional)
The form validates input but does not send email by default.
To make it functional, connect a form service:
- **Formspree:** create a form at formspree.io, set `action="https://formspree.io/f/YOUR_ID"` and `method="POST"` on the form.
- **EmailJS:** follow their docs to send emails from the frontend (no backend needed).
- **Netlify Forms:** add `netlify` attribute if deploying on Netlify.

Never put API keys or secrets in frontend code. Use environment variables on your host.

## Deploy to GitHub Pages

1. Create a new repository on GitHub (e.g. `ai-portfolio`).
2. In your project folder:
   ```
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/Joycomfort/ai-portfolio.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**.
4. Your site will be live at `https://Joycomfort.github.io/ai-portfolio/`.

## Deploy to Vercel

1. Push code to GitHub (steps above).
2. Go to vercel.com → New Project → Import your repo.
3. Framework preset: **Other** (static). Click Deploy.
4. Vercel gives you a live URL instantly.

## Three Beginner AI Projects to Build

1. **Image Classifier (CIFAR-10)** — CNN on CIFAR-10. Teaches data preprocessing, CNNs, evaluation.
2. **Sentiment Analysis** — Transformer-based text classifier. Teaches tokenization, fine-tuning.
3. **RAG Chatbot** — Document Q&A with LangChain + OpenAI/Groq. Teaches embeddings, retrieval.
4. **Data Analysis Dashboard** — Streamlit app with EDA + simple ML model. Teaches visualization, deployment.

## Portfolio Update Checklist

- [ ] Replace all placeholders with real info
- [ ] Add real project screenshots to `assets/images/`
- [ ] Update project status when completed
- [ ] Add real source/demo links
- [ ] Add certificates and hackathons as earned
- [ ] Update "Currently Learning" as you progress
- [ ] Keep skills honest (move items from Learning → Known only when confident)
- [ ] Test on mobile, tablet, and desktop
- [ ] Re-deploy after changes

## Tech Stack

- HTML5 (semantic, accessible)
- CSS3 (custom properties, responsive, dark/light theme)
- Vanilla JavaScript (no frameworks, no build step)

## License

Free to use and customize for your own portfolio.
