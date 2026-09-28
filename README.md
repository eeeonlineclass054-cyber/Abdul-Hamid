# Abdul Hamid — Portfolio Website

A clean, static, single-page portfolio built with **only HTML5 and CSS3** — no JavaScript, no frameworks, no build tools. Everything (HTML, CSS, and the profile photo) lives in one self-contained file: `index.html`.

## Files

```
index.html   → the entire site: markup, styling, and the embedded profile photo
README.md    → this file
```

## Editing the content

Everything is in one plain HTML file, so open `index.html` in any text editor and edit directly.

- **Text and sections:** all content (About, Education, Skills, Projects, Contact) is plain HTML inside `<section>` tags — just edit the text.
- **Styling:** all CSS lives inside the `<style>` block near the top of the file, organized into numbered sections (Navigation, Hero, About, Education, Skills, Projects, Contact, Footer, Responsive). Colors are defined once at the top under `:root` (e.g. `--navy-950`, `--cyan-400`) — change a value there to update it site-wide.
- **Adding a project:** find the commented-out project card template inside the Projects section, uncomment it, and fill in the title, category, description, and link (and swap in an image if you'd like). Remove the "Projects coming soon" message once you add your first real project.
- **Changing the photo:** the current photo is embedded directly as base64 text inside the `<img src="data:image/jpeg;base64,...">` tag. To swap it, convert your new image to base64 (many free online tools do this) and paste the new string in place of the old one — or simply replace it with `src="assets/your-photo.jpg"` and upload that image file alongside `index.html`.

## Deploying to GitHub Pages

1. Create a new repository on GitHub (e.g. `abdul-hamid-portfolio`).
2. Upload `index.html` to the repository root.
3. In the repository, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, select **Deploy from a branch**.
5. Choose the **main** branch and the **/ (root)** folder, then click **Save**.
6. GitHub will publish the site at:
   `https://<your-username>.github.io/<repository-name>/`
   (this can take a minute or two to go live the first time).

No build step, no npm install, and no server is required — it's ready to go as soon as the file is pushed.
