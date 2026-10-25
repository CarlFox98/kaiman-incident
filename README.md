# The Kaiman Incident — Class Action Parody Website

A parody website set up like a class action lawsuit portal for the inside joke about **The Kaiman Incident**.

## About

A joke website that looks like a law firm ("Meowfurshot Law Group") investigating a fake lawsuit about fictional bathroom incidents at furry conventions. It's set up like a real legal case portal with:

- Case overview and timeline
- Victim impact statements
- Evidence locker with viewable documents
- Public comments section
- Testimonial submission form

## Pages

| Page | Description |
|------|-------------|
| `index.html` | Home page — case overview, timeline, call to action |
| `testimonials.html` | Victim impact statements + submission form + public comments |
| `evidence.html` | Evidence locker with viewable exhibits + findings |
| `auth.html` | Log in / sign up |
| `profile.html` | Your profile |

## Usage

Live on GitHub Pages at https://carlfox98.github.io/kaiman-incident/, deployed by `.github/workflows/deploy-pages.yml` on every push to `master`.

The pages are static, with no build step. Logins, profiles, comments and testimonial submissions use a [Supabase](https://supabase.com) project. Its URL and public anon key are in `js/supabase-config.js`, and its tables are in `sql/schema.sql`. Opening the `.html` files directly still works for browsing; the logged-in features need that Supabase project.

## Disclaimer

This website is a work of parody. All characters, incidents, law firm names, and evidence are entirely fictional and created for humorous purposes among friends. No actual legal services are being offered. Any resemblance to real persons or events is purely coincidental.

## License

Do whatever you want with it.
