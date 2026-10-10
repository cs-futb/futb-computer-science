# FUTB Department of Computer Science — Website Starter

A responsive, multi-page static website starter for the Department of Computer Science at the Federal University of Technology Babura (FUTB). Built with HTML, CSS and vanilla JavaScript for GitHub Pages.

> **Important:** This repository currently contains placeholder content. It is not an official university website. Verify all departmental information and obtain the appropriate approval before publishing it as official.

## Pages included

- `index.html` — homepage
- `about.html` — department overview, vision, mission and leadership placeholders
- `staff.html` — searchable staff directory loaded from `data/staff.json`
- `staff/dr-khalid-haruna.html` — preliminary HOD profile using the supplied photograph
- `staff/sample-staff-profile.html` — individual profile template
- `programmes.html` — programme placeholders
- `research.html` — research themes and publication placeholders
- `resources.html` — student resources and useful-link placeholders
- `contact.html` — departmental contact placeholders

## Preview locally

The staff directory uses `fetch()` to load JSON, so preview with a local server rather than opening `staff.html` directly from the file system.

### Option A: Python

From the project directory, run:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

### Option B: Visual Studio Code

Install or use the Live Server extension, open the project folder and choose **Open with Live Server**.

## Publish with GitHub Pages

1. Create a repository on GitHub. For example: `computer-science-futb`.
2. Upload or push all files in this folder to the repository's default branch.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the default branch (usually `main`) and the root (`/`) folder, then save.
6. Wait for the deployment and use the URL shown in GitHub Pages settings.

The project URL will usually look like:

`https://YOUR-USERNAME.github.io/computer-science-futb/`

If the department later owns an approved GitHub organization or custom domain, update links and hosting settings accordingly.

## Update the staff directory

Edit `data/staff.json`. Each entry follows this pattern:

```json
{
  "id": "unique-staff-id",
  "name": "Full Name",
  "initials": "FN",
  "role": "Academic rank or role",
  "qualification": "Highest qualification",
  "shortBio": "Approved short biography",
  "researchInterests": ["Research area one", "Research area two"],
  "profileUrl": "staff/full-name.html"
}
```

- Use unique IDs and accurate names.
- Create a dedicated profile HTML page for each person by copying `staff/sample-staff-profile.html`.
- Use relative paths that work on GitHub Pages.
- Do not publish staff photos, personal details or biographies without appropriate authorization.
- Avoid publishing private phone numbers or personal email addresses.

## Public-source notes used in the prototype

- FUTB university overview: https://futb.edu.ng/
- School of Science, Information and Technology: https://futb.edu.ng/school-of-science-information-and-technology/
- Published university course list: https://website.futb.edu.ng/courses/
- Department seminar report (CCMAS, September 2024): https://website.futb.edu.ng/department-of-computer-science-train-staff-on-ccmass-implementation/

The Computer Science programme is present in the published course list. The Artificial Intelligence programme's mid-2026 approval and expected 2027 start are based on a departmental update supplied for this prototype; the public course list checked during preparation did not yet list AI. Verify this with the department before public launch. The homepage's research themes are presented as broad areas of interest, not claims of existing labs or funded projects.

## Public-source notes used in the prototype

- FUTB university overview: https://futb.edu.ng/
- School of Science, Information and Technology: https://futb.edu.ng/school-of-science-information-and-technology/
- Published university course list: https://website.futb.edu.ng/courses/
- Department seminar report (CCMAS, September 2024): https://website.futb.edu.ng/department-of-computer-science-train-staff-on-ccmass-implementation/

The Computer Science programme is present in the published course list. The Artificial Intelligence programme's mid-2026 approval and expected 2027 start are based on a departmental update supplied for this prototype; the public course list checked during preparation did not yet list AI. Verify this with the department before public launch. The homepage's research themes are presented as broad areas of interest, not claims of existing labs or funded projects.

## Public-source notes used in the prototype

- FUTB university overview: https://futb.edu.ng/
- School of Science, Information and Technology: https://futb.edu.ng/school-of-science-information-and-technology/
- Published university course list: https://website.futb.edu.ng/courses/
- Department seminar report (CCMAS, September 2024): https://website.futb.edu.ng/department-of-computer-science-train-staff-on-ccmass-implementation/

The Computer Science programme is present in the published course list. The Artificial Intelligence programme's mid-2026 approval and expected 2027 start are based on a departmental update supplied for this prototype; the public course list checked during preparation did not yet list AI. Verify this with the department before public launch. Homepage research themes are broad areas of academic interest, not claims of existing labs or funded projects.

## Content checklist before launch

- [ ] Confirm official department name, history, vision, mission and leadership.
- [ ] Verify current staff list, ranks, qualifications and approved contact details.
- [ ] Verify programme availability, accreditation status, admissions information and curriculum.
- [ ] Verify publication metadata, author names, DOI links and research claims.
- [ ] Add official university links and current approved student resources.
- [ ] Replace all sample names and bracketed fields.
- [ ] Add approved logo, staff photographs and image credits where needed.
- [ ] Test every link, the staff search, keyboard navigation and mobile layouts.
- [ ] Confirm departmental/university authorization and agree who maintains the repository.

## Technical notes

- No build step or package manager is required.
- The site uses a Google Fonts import for DM Sans and Manrope. If you want fully self-contained/offline styling, remove the `@import` line in `assets/css/style.css` and use system fonts.
- The contact page is informational only; it does not submit messages.
- GitHub Pages is static hosting. A content management system or backend would be needed for a secure staff login and browser-based content editing.
