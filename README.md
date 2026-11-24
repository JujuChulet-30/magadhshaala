# MagadhShala (मगधशाला)

A responsive, bilingual (English/Hindi) static website prototype for a Bihar-focused school learning and resource hub.

## Pages

- `index.html` — public landing page and portal directory
- `student.html` — student activity library, grade filters, progress tracker and demo project submission form
- `teacher.html` — teacher resource centre
- `leadership.html` — school leadership hub

## Technology

- HTML5
- CSS3
- Vanilla JavaScript
- Browser `localStorage` for language preference, activity completion and demo submissions
- No build step, package manager, API key or server required

## Run locally

Open `index.html` in a browser. For a local web server, run:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

## Deploy to GitHub Pages

1. Create a public GitHub repository named `magadhshala`.
2. Upload the **contents** of this folder to the repository root. `index.html`, `app.js` and `styles.css` must be in the root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Choose branch `main` and folder `/(root)`, then save.
6. GitHub Pages will publish the site at `https://YOUR-USERNAME.github.io/magadhshala/`.

## Language switching

The language selector is available on every page. It switches all page copy, navigation, labels, notices, form text, dynamic activity cards and resource descriptions between English and Hindi. The selected language is saved in `localStorage` under `magadhshala_language`, so it remains selected while navigating between pages in the same browser.

To reset the language, clear the site's local storage or run this in the browser console:

```js
localStorage.removeItem('magadhshala_language');
location.reload();
```

## Prototype limitations and production requirements

- Activity completion and project submission are stored only in the current browser. They are not sent to a school or central dashboard.
- Resource links are demonstration interactions. Replace them with approved, accessible learning materials.
- There is no login, role-based access, central database, file upload service, analytics backend or administrator dashboard.
- Sample activities are illustrative and are not represented as an approved Bihar Board or SCERT curriculum.
- Before collecting identifiable student or teacher information, implement consent, data minimisation, security, retention and authorised hosting requirements.
- This is an independent prototype and is not an official Government of Bihar website.

## Suggested next development phase

1. Validate content against Bihar SCERT and relevant programme requirements.
2. Conduct usability testing with students, teachers and school leaders.
3. Define authentication and roles.
4. Add an approved backend and database.
5. Add central submissions, reporting and district-level dashboards.

## License

See `LICENSE`.
