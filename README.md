# BiharShala — Bihar School Learning Hub

A responsive, static website prototype for a proposed school learning and resource portal for Bihar. It is inspired by the broad information architecture of DigiShaala's CBSE hub (role-based portals, student activities, teacher resources and submissions), but uses original branding, layout, copy and code.

**Status:** Front-end prototype / pre-work demonstration. Not an official Government of Bihar, Bihar Board, SCERT or education department platform.

## Live demo locally

No build tools, package manager or server are required.

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Navigate to Student, Teacher and School Leadership portals.

For a local web server, run `python3 -m http.server 8000` in the project directory and visit `http://localhost:8000`.

## Included functionality

- Responsive landing page and role-based navigation.
- Student portal with sample activities, grade filters, search and completion checklist.
- Student completion state stored in browser `localStorage`.
- Student project submission demo form; submissions are stored only in that browser's `localStorage`.
- Teacher resource centre and school leadership resource hub.
- Mobile navigation and date/year display.
- Basic English/Hindi toggle on the landing page.

## Important limitations

This is a static GitHub Pages prototype. It does **not** include user accounts, central database, secure file uploads, school verification, admin dashboard, analytics, real-time sync, certificates or a working central submission workflow. The form data is not sent to a server. Resource entries are examples and do not represent official curriculum or approved government material. Do not collect real student personal data through this prototype.

For production, plan an authenticated backend, role-based access, secure storage, consent and privacy notices, audit logs, backup, moderation and an authorised data governance owner. Verify all Bihar curriculum alignment and resource links with the relevant education authority before publishing.

## Deploy to GitHub Pages

1. Sign in to GitHub and create a new **public** repository, for example `biharshala`.
2. Keep the repository empty (do not initialise with a README if you plan to upload this folder as-is).
3. On your computer, unzip the project. Open Terminal in the `biharshala` folder.
4. Run:

   ```bash
   git init
   git add .
   git commit -m "Initial BiharShala website prototype"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/biharshala.git
   git push -u origin main
   ```

5. In the repository, open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select branch **main** and folder **/(root)**, then click **Save**.
8. Wait for the Pages deployment to finish. Your site will be available at:

   `https://YOUR-USERNAME.github.io/biharshala/`

9. Test the homepage and all three portal links on desktop and mobile.

### Alternative: upload through GitHub website

Create the repository → **Add file → Upload files** → drag all files and folders from this project into the upload area → commit to `main` → configure Settings → Pages as above.

## Suggested next development phases

1. Confirm name, identity, target grades, language and content ownership.
2. Map activities and resources to approved Bihar curriculum and programme priorities.
3. Add school/district metadata and role-based sign-in.
4. Build backend APIs, database, file storage and admin workflows.
5. Add dashboards, reporting, consent/privacy controls and accessibility testing.
6. Pilot with a small set of schools before statewide rollout.

## Project structure

```text
biharshala/
├── index.html          # Landing page
├── student.html        # Student portal
├── teacher.html        # Teacher resource centre
├── leadership.html     # School leadership hub
├── styles.css          # Shared responsive design system
├── app.js              # Navigation, filters, progress and demo form logic
├── README.md           # Setup, deployment and limitations
└── LICENSE             # MIT license for this original prototype code
```

## Customisation

- Replace sample activities in `app.js` with approved activity records.
- Replace resource placeholders in `app.js` with approved document URLs and descriptions.
- Update page text and visual identity in the HTML/CSS files.
- If adding real student accounts or submissions, do not use `localStorage` as a substitute for a secure backend.

## Credits and naming

BiharShala is a proposed working name only. Check trademark, domain and social handle availability before adopting it formally. This project is an independent prototype and is not affiliated with DigiShaala, Adobe, CBSE or the Government of Bihar.
