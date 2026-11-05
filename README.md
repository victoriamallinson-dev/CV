# CV

A markdown-driven academic CV, built with Jekyll and hosted on GitHub Pages.

## Editing your CV

All the content lives in **`index.md`**. Each section has:

- A red *hint* line (in italics) explaining what goes there — delete it once you've filled the section in.
- One or two example entries showing the formatting to copy.

Sections included (in order): Currently, Education, Research experience, Teaching
experience, Papers, Grants, Awards, Presentations (Invited / Submitted), Outreach,
Involvement, Mentoring, Media, Technical skills and languages, Areas of experience,
Projects, References.

Update the name, tagline, affiliation and contact line at the top of `index.md`,
then work through each section, deleting the hint and example rows as you add your
own entries.

### Formatting cheat sheet

- **Dated entry** (Education, Awards):
  ```markdown
  2024
  : Description of the entry
  {: .entry}
  ```
- **Citation-style entry** (Papers, Presentations, Media) — hanging indent, bold your own name:
  ```markdown
  **Your Last Name, F.**, Co-author, A. (Year). Title. *Journal*, pages.
  {: .pub}
  ```
- **Role/appointment line** (Research/Teaching experience, Outreach, Involvement, Mentoring):
  ```markdown
  Role – Organization [dates]
  {: .appt}
  ```
- **Multi-column list** (Skills, Areas of experience):
  ```markdown
  - Item one
  - Item two
  {: .columns}
  ```

## Previewing locally

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Publishing with GitHub Pages

1. Push this repo to GitHub.
2. In the repo's **Settings → Pages**, set the source to the branch you want
   published (e.g. `main`) and the root folder.
3. GitHub Pages builds the Jekyll site automatically — no extra config needed.

## Printing / saving as a PDF

Open the published page and click **Print / Save as PDF** (top right), or use your
browser's print dialog. A separate print stylesheet (`assets/css/cv-print.css`)
produces a clean, compact PDF layout and hides the editing hints automatically.
