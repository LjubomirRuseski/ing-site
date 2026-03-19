# Inginstitut Website Improvement Plan

**Prepared for:** Ингинститут (inginstitut.com)
**Date:** March 2026
**Scope:** Full website redesign and content strategy

---

## Executive Summary

The current website is essentially a placeholder — three short paragraphs, no navigation, no contact form, and a note saying "the site is under construction." This significantly undersells a business with 50+ accredited experts across 11 disciplines. The redesigned prototype (index.html) addresses all major gaps identified below.

---

## 1. What's Wrong With the Current Site

### Design & Structure
- No navigation menu — visitors cannot jump between sections
- No visual hierarchy — everything reads like one flat block of text
- No call-to-action buttons (nothing prompts a visitor to take the next step)
- The hero section has a dated look: a basic bordered text box on a dark background
- No mobile responsiveness beyond the default browser rendering
- No footer with real information

### Content & Credibility
- The "under construction" message destroys credibility immediately — it signals the business hasn't invested in its online presence
- The 50+ experts are never mentioned specifically; there are no profiles, no names, no credentials
- The 11 disciplines are listed as one long comma-separated sentence — easy to miss
- No "why us" section or differentiators — why would a client choose Inginstitut over another veštak?
- No testimonials, case studies, or social proof of any kind

### Functionality
- No contact form — visitors must copy/paste an email address and leave the site
- No phone number or physical address
- No language option (potential for international clients, EU institutions, etc. is untapped)
- No SEO metadata (title tags, descriptions, structured data)

---

## 2. What the Redesign Addresses

### Structure (New Sections)
| Section | Purpose |
|---|---|
| **Fixed Navbar** | Persistent navigation with smooth scroll and language toggle |
| **Hero** | Strong first impression with headline, subtext, CTAs, and key stats |
| **About** | Trust-building overview with a visual stat highlight |
| **Services** | 6 distinct service cards — easy to scan |
| **Disciplines** | 11 discipline tiles with icons — scannable at a glance |
| **Why Inginstitut** | 4 key differentiators in a visually distinct dark section |
| **Contact** | Contact info sidebar + full inquiry form |
| **Footer** | Clean, professional closing |

### Visual Design
- Professional navy/gold colour palette consistent with legal and institutional trust
- Clean typography with clear size hierarchy
- Hover states and subtle animations for interactivity
- Consistent card-based layout with border accents
- Mobile-responsive grid layouts

### Bilingual Support
- MK / EN toggle in the navbar
- All copy translated and toggled via `data-lang` attribute on `<body>`
- No page reload required — instant toggle

---

## 3. Next Steps (Priority Order)

### Immediate (Do Before Launch)

**3.1 Fill in real contact details**
Replace the placeholder contact information with:
- Full street address (helps with local SEO and builds trust)
- Phone number
- Working hours (already templated in the design)

**3.2 Add an expert directory**
The single biggest trust signal you can add is a page (or section) listing your experts. Even basic profiles work:
- Name and title
- Discipline(s)
- Years of experience
- Accreditation/licence number (optional)

This transforms the site from "we have experts" to "here are the specific people who will help you."

**3.3 Connect the contact form to a real backend**
The current form shows a success message but doesn't actually send anything. Options:
- Use a free service like **Formspree** (formspree.io) — just change the `<form action>` attribute
- Use **EmailJS** for client-side email sending with no backend
- Use a backend form handler on your server

**3.4 Replace the "© 2025" with the correct year** (currently 2025 in the template — update to match your launch year).

---

### Short-Term (Within 1–3 Months)

**3.5 SEO basics**
- Add structured data (Schema.org `LocalBusiness` and `LegalService` markup)
- Submit to Google Search Console
- Create a Google Business Profile for local search visibility
- Add alt text to any images you add later

**3.6 Add a case studies or results section**
Even 2–3 anonymised examples ("We provided forensic expertise in a construction dispute — the court accepted our findings and the client won") build significant credibility.

**3.7 Add testimonials**
Reach out to past clients (law firms, companies) for a short quote. A few lines from a lawyer saying "Inginstitut's reports are always thorough and accepted by the court" is worth more than any marketing copy.

**3.8 Professional photography**
A team photo or a photo of your office/working environment adds significant warmth and credibility to the "About" section.

---

### Medium-Term (3–6 Months)

**3.9 Individual service pages**
Each of the 6 service types (forensic expertise, super-expertise, consulting, etc.) deserves its own page with:
- Detailed description
- What the process looks like (step by step)
- Typical timeline and deliverables
- Relevant disciplines
- A specific contact form

**3.10 Expert sub-pages by discipline**
Group experts by discipline with individual profile pages. This dramatically improves SEO for searches like "вешто лице за градежништво Македонија" (forensic expert for construction Macedonia).

**3.11 Blog or resources section**
Publishing 1–2 articles per month on topics like "How forensic expertise works in Macedonian courts" or "What to expect from a super-expertise review" builds authority and drives organic traffic.

---

## 4. Technical Hosting Recommendations

If you don't already have a hosting setup, here are simple options:

| Option | Cost | Best For |
|---|---|---|
| **Netlify** (netlify.com) | Free tier available | Dropping a single HTML file, no backend needed |
| **GitHub Pages** | Free | Static sites, version-controlled |
| **Hetzner** (hetzner.com) | ~€4/mo | Affordable VPS, good for European businesses |
| **WordPress + hosting** | ~€5–15/mo | If you want a CMS to update content easily without coding |

For the short term, the single HTML file provided can be deployed to Netlify in under 5 minutes by dragging and dropping the file into their dashboard.

---

## 5. Summary of Key Improvements

| Area | Before | After |
|---|---|---|
| Navigation | None | Fixed navbar with smooth scroll |
| Hero | Static box with title | Headline + description + CTAs + stats |
| Services | 2 paragraphs | 6 visual service cards |
| Disciplines | Comma-separated list | 11 icon tiles |
| Social proof | None | Stats, "Why Us" section, room for testimonials |
| Contact | Email address only | Form + email + hours + location |
| Language | Macedonian only | MK / EN toggle |
| Mobile | Not optimised | Responsive grid layouts |
| SEO | No meta tags | Title, description, lang attributes |

---

*This document was prepared based on analysis of the live site at www.inginstitut.com as of March 2026.*
