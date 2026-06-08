# PacketCheck Landing Page

## Purpose

This directory contains a simple consumer-facing landing page for PacketCheck. It is intended to test whether borrowers understand the problem PacketCheck addresses and find the proposed checklist useful.

The page focuses on the experience of organizing mortgage documents after a lender asks for them.

## Preview Locally

```bash
cd site
python3 -m http.server 8080
```

Open:

```text
http://localhost:8080
```

## GitHub Pages

The repository includes `.github/workflows/pages.yml`, which publishes the static landing page after changes reach the `main` branch.

Expected public URL:

```text
https://sourabhmarathe.github.io/packetcheck/
```

## Waitlist Form

The early-access form currently submits to this placeholder endpoint:

```text
https://example.com/waitlist-form-endpoint
```

A real form provider endpoint must replace this URL before publishing the page. The current endpoint is intentionally non-production and will not create a working waitlist.

The form is limited to an email address, a short audience-selection field, and an optional description of the borrower's paperwork problem. The page does not collect or upload mortgage documents. Its privacy warning tells visitors not to submit Social Security numbers, bank account numbers, or other sensitive financial information.

## Files

- `index.html`: page structure and copy
- `styles.css`: responsive visual design
- `README.md`: preview and maintenance notes

## Technical Notes

There is no build step. The page uses plain static HTML and CSS with no JavaScript, external fonts, frameworks, analytics, backend, or external assets.
