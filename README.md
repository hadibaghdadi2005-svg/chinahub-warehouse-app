# ChinaHub Warehouse

The staff app for a China → Lebanon consolidation warehouse: sign in, look a
parcel up, and — for an admin — decide who may do what.

This repository is public only because GitHub Pages needs it to be. It holds
the page and its icons, nothing else. There is no customer data here and never
should be: names, phone numbers, charges and payment status live in the
database, behind row-level security, and are only ever read by someone signed
in with a role.

The key in `index.html` is a Supabase *publishable* key. It is meant to sit in
client code. On its own it opens nothing — every table refuses an account that
has no profile, and the money columns are masked for anyone below office.

Built from the private working repository; this copy is generated, so edit it
there rather than here.
