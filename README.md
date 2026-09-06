# Curricular Student Leadership — ASCEND MD

Single-file page (`index.html`). All student photos are embedded (base64), so nothing else is required for it to render.

## Deploy
Upload the `student-leadership/` folder to the `sinaiascend.github.io` repo. It will be live at
`https://sinaiascend.github.io/student-leadership/`.

Optional: copy `assets/icahn-logo.png` from the org-chart app into `student-leadership/assets/` to show the
Icahn logo in the top bar (a text lockup is used until then).

## Editing
Open `index.html` and edit the `DATA` object near the top of the `<script>`:
- Add/remove people with `P("First Last")` (optional tag: `P("First Last","M2")`).
- Mark a module/clerkship without reps as `{ name: "...", pending: true }`.
- Groups and people sort alphabetically automatically.

## Adding a photo for someone not embedded
Drop `student-leadership/assets/students/firstname-lastname.jpg` (lowercase, accents stripped).

## PDF
`student-leadership.pdf` is the roster-style photo grid linked from the "Download PDF" buttons. It is generated
separately from `index.html`; send the updated `index.html` to Claude to regenerate it after roster changes.
