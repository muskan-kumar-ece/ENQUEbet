# ENQUEbet — Where Ideas Take Off 🚀

[![Website](https://img.shields.io/website?url=https%3A%2F%2Fenquebet.vercel.app&label=Live%20Site&style=flat-square)](https://enquebet.vercel.app)
[![Deployed on Vercel](https://img.shields.io/badge/Deployed%20on-Vercel-black?style=flat-square&logo=vercel)](https://vercel.com)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)

---

## About the Project

**ENQUEbet** is the official website of the student innovation club based at **MRCET, Hyderabad**. It serves as the digital hub for creators, coders, designers, and thinkers to **propose ideas, discover projects, join events, collaborate with peers, and get mentored** by faculty and industry professionals.

The platform was born from a single question: *"What if students had a place to actually build things that matter?"* ENQUEbet is that launchpad — connecting 1,200+ students across disciplines to turn bold ideas into real-world impact.

> **Live site:** [https://enquebet.vercel.app](https://enquebet.vercel.app)

---

## Key Features

- 🚀 **Idea Submission** — Students can submit their project ideas through a dedicated form.
- 🤝 **Collaboration Hub** — Connect with other clubs, join open-source projects, and find teammates.
- 🗓️ **Events Calendar** — Browse and register for upcoming bootcamps, hackathons, and workshops.
- 🏆 **Achievements Gallery** — Showcases club awards, patents, and competition wins.
- 💡 **Ideas Gallery** — Explore a browsable archive of student-submitted ideas for inspiration.
- 🛠️ **Projects Showcase** — Highlighted student projects with descriptions and outcomes.
- 📰 **Blog & Articles** — Student writeups, tech trends, and innovation stories.
- 👥 **Team & Mentors** — Meet the student leaders, alumni, and faculty coordinators.
- 🔬 **Labs & Resources** — Interactive cards for the AI/ML Lab, IoT Lab, Design Studio, and Startup Support.
- 📱 **Fully Responsive** — Mobile-first design with a hamburger menu and adaptive layouts.
- ⏱️ **Live Event Countdown** — Real-time countdown timer for the next upcoming event.
- ✨ **Smooth Animations** — AOS (Animate On Scroll) library for polished scroll-triggered reveals.
- 🔍 **SEO-Optimised** — Canonical tags, meta descriptions, `sitemap.xml`, and `robots.txt` included.

---

## Tech Stack

| Category       | Technology / Tool                                                    |
|----------------|----------------------------------------------------------------------|
| **Markup**     | HTML5 (semantic, multi-page)                                         |
| **Styling**    | Vanilla CSS3 (`style.css`, `theme-override.css`), Google Fonts (Inter) |
| **Scripting**  | Vanilla JavaScript ES6+ (`main.js`, `navbar.js`)                    |
| **Animations** | [AOS 2.3.4](https://michalsnik.github.io/aos/) (Animate On Scroll)  |
| **Icons**      | [Font Awesome 6.4.0](https://fontawesome.com/)                       |
| **Images**     | [Cloudinary](https://cloudinary.com/) (external CDN hosting)        |
| **Deployment** | [Vercel](https://vercel.com) (static site hosting)                  |
| **SEO**        | `sitemap.xml`, `robots.txt`, Google Site Verification               |

> **No build tools, no frameworks, no dependencies to install.** This is a pure static website — open `index.html` in a browser and it works.

---

## Folder Structure

```
ENQUEbet/
│
├── index.html              # Home page — hero, project carousel, labs, testimonials
├── about.html              # About Us — mission, team, journey, testimonials
├── projects.html           # Projects showcase
├── events.html             # Upcoming events & registration
├── ideas.html              # Ideas gallery (student submissions)
├── submit.html             # Idea submission form
├── blog.html               # Blog & articles
├── team.html               # Full team & mentors page
├── achievements.html       # Awards, patents, hackathon wins
├── collab.html             # Collaboration hub
├── centerofcollab.html     # Center of Collaboration landing
├── contact.html            # Contact form & details
├── privacy.html            # Privacy policy
├── terms.html              # Terms of service
├── logo-snippet.html       # Reusable logo HTML snippet
│
├── style.css               # Global stylesheet (design system, components, layout)
├── theme-override.css      # Light theme overrides and custom variables
│
├── main.js                 # Site-wide scripts (AOS init, countdown, counters, smooth scroll)
├── navbar.js               # Responsive navigation (toggle, keyboard, accessibility)
│
├── photos/
│   └── sitelogo.png        # Club logo asset
│
├── sitemap.xml             # XML sitemap for search engine indexing
└── robots.txt              # Crawler directives
```

---

## Getting Started (Local Setup)

Since ENQUEbet is a **zero-dependency static website**, setup is extremely simple and requires no package installation.

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- *(Optional)* [VS Code](https://code.visualstudio.com/) with the **Live Server** extension, or any local HTTP server, for the best development experience.

> **Note:** You can open `index.html` directly in a browser (via `file://`) and all pages will work. A local server is recommended only because some browser security policies restrict certain features on `file://` URLs.

---

### 1 · Clone the Repository

```bash
git clone https://github.com/enquebet/ENQUEbet.git
cd ENQUEbet
```

---

### 2 · Open the Site Locally

**Option A — Direct file open (simplest):**

```bash
# Windows
start index.html

# macOS
open index.html

# Linux
xdg-open index.html
```

**Option B — VS Code Live Server (recommended):**

1. Open the project folder in VS Code.
2. Install the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension.
3. Right-click `index.html` → **Open with Live Server**.
4. The site opens at `http://127.0.0.1:5500`.

**Option C — Python simple HTTP server:**

```bash
# Python 3
python -m http.server 8000
```
Then navigate to `http://localhost:8000`.

---

### 3 · Environment Variables

This is a static frontend-only site. There are **no environment variables** required to run it locally.

If you extend this project to include a backend (e.g., for form submissions or a CMS), you would need something like:

| Variable                | Description                                  |
|-------------------------|----------------------------------------------|
| `[FORM_ENDPOINT_URL]`   | Endpoint for the idea/contact submission form |
| `[CLOUDINARY_CLOUD_NAME]` | Cloudinary account name for image uploads   |
| `[GOOGLE_ANALYTICS_ID]` | GA4 Measurement ID for analytics             |

---

### 4 · Making Changes

All pages follow the same structure. To edit content:

- **Page content** → Edit the corresponding `.html` file.
- **Global styles** → Edit `style.css`.
- **Theme colours/overrides** → Edit `theme-override.css`.
- **Site-wide behaviour** → Edit `main.js`.
- **Navigation behaviour** → Edit `navbar.js`.
- **SEO metadata** → Update the `<meta>` tags in each HTML `<head>` and `sitemap.xml`.

---

## Usage

Once the site is running, here are the main entry points:

| Page | URL / File | Purpose |
|------|------------|---------|
| Home | `index.html` | Hero, stats, project carousel, labs, event countdown |
| Submit Idea | `submit.html` | Form for students to submit project ideas |
| Join the Club | `contact.html` | Contact form, social links, membership |
| Projects | `projects.html` | Browse all student-built projects |
| Events | `events.html` | Upcoming workshops, bootcamps, hackathons |
| Ideas Gallery | `ideas.html` | Explore submitted student ideas |
| Blog | `blog.html` | Articles and student writeups |
| Team | `team.html` | Faculty coordinators and student leaders |
| Achievements | `achievements.html` | Awards, patents, recognition |

> **Admin access:** This site has no admin panel or CMS — all content is managed directly by editing the HTML files and committing to the repository.

---

## Deployment

The site is deployed on **Vercel** with automatic deployments on every push to the `main` branch.

To deploy your own fork:

1. Fork this repository on GitHub.
2. Go to [vercel.com](https://vercel.com) and import your forked repository.
3. Vercel will auto-detect it as a **Static Site** — no build command or output directory configuration needed.
4. Click **Deploy**. Done.

---

## Contributing

Contributions are welcome! Whether it's fixing a typo, improving accessibility, adding a new section, or updating club information — all help is appreciated.

### How to Contribute

1. **Fork** this repository.
2. **Create a branch** for your feature or fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes** — keep them focused and well-tested in the browser.
4. **Commit** with a clear message:
   ```bash
   git commit -m "feat: add [description of change]"
   ```
5. **Push** to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```
6. Open a **Pull Request** against the `main` branch of this repository and describe your changes.

### Guidelines

- Keep the design consistent with the existing colour palette (`#6a82fb`, `#fc5c7d`, `#43cea2`).
- Test all pages at both mobile (`< 700px`) and desktop widths before submitting.
- Ensure any new images are hosted on Cloudinary or another CDN (avoid committing large binary assets).
- Run the site through [PageSpeed Insights](https://pagespeed.web.dev/) and aim to maintain a high performance score.

---

## Contact

| Channel | Details |
|---------|---------|
| **Email** | fluxedustart@gmail.com |
| **Phone** | +91 6302812452 |
| **Address** | ENQUEbet, MRCET, Hyderabad |
| **Instagram** | [@enquebet](https://www.instagram.com/enquebet/) |
| **GitHub** | [github.com/enquebet](https://github.com/enquebet) |

---

<div align="center">

© 2025 ENQUEbet. All Rights Reserved. &nbsp;|&nbsp; [Privacy Policy](privacy.html) &nbsp;|&nbsp; [Terms of Service](terms.html)

*Empowering student innovators to build the future.*

</div>

