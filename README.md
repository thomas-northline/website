# Northline Infrastructure — GitHub Pages site

A responsive, static consulting website built with plain HTML, CSS, and JavaScript. No build tools or dependencies are required.

## Preview locally

Open `index.html` in a browser, or from the project folder run a simple local server:

```powershell
py -m http.server 8000
```

Then visit `http://localhost:8000`.

## Deploy to GitHub Pages

1. Create a new GitHub repository, for example `northline-infrastructure`.
2. Upload `index.html`, `styles.css`, `script.js`, and `README.md` to the repository root.
3. In GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main` and folder `/ (root)`, then click **Save**.
6. Wait for GitHub Pages to publish the site. The URL will appear on the Pages settings screen.

You can also push the files using Git:

```powershell
git init
git add .
git commit -m "Build Northline consulting website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/northline-infrastructure.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username and ensure the repository URL matches the repository you created.

## Before publishing

- Update `hello@northlineinfrastructure.com` in `index.html` if you want a different contact address.
- Review the service descriptions and confirm they accurately represent the services you intend to offer.
- Add your own privacy notice if you later introduce analytics, tracking, or a form service.

## Contact form note

The contact CTA currently opens the visitor's default email app with a prefilled subject. GitHub Pages serves static files and does not process form submissions by itself. If you want a true web form, connect a form provider or a small backend later.
