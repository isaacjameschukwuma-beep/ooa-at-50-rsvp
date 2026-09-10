# OOA at Fifty — RSVP

A single-page invitation and RSVP for Mr Shola Ajayi's 50th.

- **When** Friday, 11 September 2026, 10:00 WAT
- **Where** The Nest Gardens, Bala Muhammed Way, Guzape, Abuja
- **Colour of the day** White

## How it works

`index.html` is the whole site. No build step, no dependencies. The invitation
card is embedded in the page as a data URI, so there are no external assets to
host. Fonts come from Google Fonts.

Guests enter a name, choose whether they are attending, and are handed two
actions: a prefilled WhatsApp reply to the family, and a Google Calendar link.

## Deploying

Vercel serves `index.html` at the root with no configuration. Import this
repository as a new project and accept the defaults; leave the build command
and output directory empty.

## Editing

Two values near the top of the `<script>` block are meant to be changed:

- `RSVP_PHONE` — the WhatsApp line replies are sent to.
- `FORM_ENDPOINT` — optional. Paste a Formspree or Getform URL here to also
  receive a copy of every RSVP by email. Left empty, replies arrive only
  through WhatsApp.
