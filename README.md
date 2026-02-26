# Highlight Digital Business Card (Blinq-like)

## What this is
A lightweight, static, Blinq-style digital business card system:
- Desktop layout with employee search + Save to Contacts + Send to Phone (QR + share options)
- Mobile layout with QR under the photo + Save / Share / Find
- Forced mobile view link: `?view=mobile` (works even on Mac/PC)
- Employee selection via `?u=employee-id`

## Quick start (GitHub Pages)
1. Create a new GitHub repo and upload these files.
2. In GitHub: Settings → Pages → Deploy from branch → `main` → `/ (root)`.
3. Your link will look like: `https://<username>.github.io/<repo>/`

## URLs
- Desktop (auto): `/index.html?u=jessica-flanders`
- Forced mobile (for QR codes): `/index.html?u=jessica-flanders&view=mobile`

## Add employees
Edit `employees.json` and add a new object:
- `id` must be URL-safe (use dashes).
- `photo` can be null — it will use `fallbackPhoto` (building image).

## Notes
QR codes are generated using a hosted QR image endpoint.
If you want fully-offline QR generation later, we can swap in a tiny local JS QR library.
