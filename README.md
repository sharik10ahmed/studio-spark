# Studio Spark

https://github.com/sharik10ahmed/d-maker-flow

copy this repo and start where it was left off 

initial prompt

Done

All 31 unique images generated in src/assets/ (hero, about, 6 programs, 7 fitness, choreography, 5 events, 10 gallery) — no image is reused anywhere.

Design system in src/styles.css: Electric Orange / charcoal / white / soft-gray tokens, Anton + Plus Jakarta Sans families, reveal / hero-pan / marquee utilities.

Data layer: src/data/images.ts (single-registration image registry), src/data/mock.ts (programs, fitness, choreography, gallery, events, testimonials, enquiries, settings, why-us, process, stats, mock admin credentials).

State layer: src/store/studio.tsx — generic collection CRUD (add/update/delete/toggle), settings updates, enquiry submission, mock admin login/logout. No backend, no database.

UI primitives: Button, Icon (inline SVGs, no icon library), Reveal, SectionHeading, Modal.

Current situation

Done

All 31 unique images generated in src/assets/ (hero, about, 6 programs, 7 fitness, choreography, 5 events, 10 gallery) — no image is reused anywhere.

Design system in src/styles.css: Electric Orange / charcoal / white / soft-gray tokens, Anton + Plus Jakarta Sans families, reveal / hero-pan / marquee utilities.

Data layer: src/data/images.ts (single-registration image registry), src/data/mock.ts (programs, fitness, choreography, gallery, events, testimonials, enquiries, settings, why-us, process, stats, mock admin credentials).

State layer: src/store/studio.tsx — generic collection CRUD (add/update/delete/toggle), settings updates, enquiry submission, mock admin login/logout. No backend, no database.

UI primitives: Button, Icon (inline SVGs, no icon library), Reveal, SectionHeading, Modal.

Remaining

Two build errors to fix first: use paths["sparkles"] in Icon.tsx, and rename my ui/Button.tsx to avoid the casing clash with the template's existing ui/button.tsx (e.g. move mine to src/components/ui/ActionButton.tsx).

Site components: Header (sticky/compact, mobile drawer), Footer (with the subtle Admin Login link), Hero + animated stats, Program/Fitness/Choreography/Event/Testimonial cards, GalleryGrid with filtering + lightbox, Why Us, Training Process timeline, CTA section, ContactForm.

Public routes: /, /about, /programs, /fitness, /choreography, /gallery, /events, /testimonials, /contact, each with its own head() metadata; replace the placeholder index.

Admin: /admin/login plus /admin dashboard and the programs, fitness, choreography, gallery, events, testimonials, enquiries and settings modules, sharing an AdminShell (responsive sidebar drawer) and a generic resource manager with DataTable + modal forms.

Wrap the app in StudioProvider and load the fonts via <link> in src/routes/__root.tsx.

This project was built with [Lovable](https://lovable.dev).

## Build with Lovable

Continue developing this project in the [Lovable editor](https://lovable.dev/projects/84cd2267-827b-4a1e-9c8e-8ea4b3a49ffe).

- **Ship faster**: describe what you want to build and Lovable handles the code.
- **Stay in sync**: every change made in Lovable is committed straight to this repository.
- **Full ownership**: this code is yours. Push to `main` on GitHub and your changes sync back into Lovable, ready for your next prompt.

## Development

Prefer working locally? You need Node.js and npm — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating).

```sh
git clone <this-repository-url>
cd <repository-name>
npm i
npm run dev
```
