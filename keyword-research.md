# VibeCV — SEO Keyword Research

Base domain: `https://vibecv.com`. Derived from listing data in [app.md](app.md), competitive App Store Optimization (ASO) terms, and organic search intent for the resume-builder category. Prioritized for **download intent** (transactional/commercial) over pure informational volume.

## Primary Keywords (head terms — target on homepage title, H1, meta)

| Keyword | Intent | Why it converts |
|---|---|---|
| AI resume builder | Commercial | Highest-intent 2-word term combining the app's core differentiator (AI) with the category |
| resume builder app | Commercial | Mobile-first buyer intent, matches "app" qualifier used by people ready to download |
| ATS resume checker | Commercial | Unique feature term with lower competition than "resume builder," strong buyer intent |
| free resume builder | Commercial | High volume, "free" qualifier filters in price-sensitive downloaders |
| CV maker app | Commercial | Captures international/non-US traffic where "CV" outranks "resume" |
| ATS friendly resume templates | Commercial | Feature + fear-based intent (rejection avoidance) drives clicks |
| resume builder for freshers | Commercial | Underserved, high-conversion niche (India/APAC market where "fresher" is standard terminology) |
| best resume app | Comparison | Captures users actively comparing apps right before download |

## Long-Tail Keywords (guide pages — informational-to-transactional, lower competition, high conversion)

Each maps to one dedicated guide in `/guides/` that answers the query directly, then converts into an app download.

| # | Long-tail keyword | Search intent | Guide slug |
|---|---|---|---|
| 1 | how to check ats score of resume for free | "Am I going to get filtered out?" anxiety search | `guides/check-ats-score-free.html` |
| 2 | why does my resume get rejected by ats | Same anxiety cluster, higher volume, pairs with #1 | `guides/fix-resume-ats-rejection.html` |
| 3 | best resume builder app for freshers | Comparison + first-job urgency | `guides/best-resume-builder-for-freshers.html` |
| 4 | free ats friendly resume templates | Template-shopping, very high volume | `guides/ats-friendly-resume-templates.html` |
| 5 | how to make a resume on your phone | Mobile-only users, no laptop access | `guides/make-a-resume-on-your-phone.html` |
| 6 | how to write a resume with ai | Tool-curious, wants speed | `guides/write-a-resume-with-ai.html` |
| 7 | resume builder for students with no experience | Zero-experience anxiety, huge underserved segment | `guides/resume-builder-for-students.html` |
| 8 | how to add keywords to resume for ats | Tactical/actionable, high buyer intent | `guides/add-keywords-to-resume-for-ats.html` |
| 9 | best cv maker app for iphone and android | Cross-platform comparison shopper | `guides/best-cv-maker-app.html` |
| 10 | resume builder for career change | Life-event triggered search, freelancers/switchers | `guides/resume-builder-for-career-change.html` |

### Why these ten

- Every keyword contains a **verb or comparison modifier** ("how to," "best," "free") — these outrank single-noun head terms in AI Overviews and featured snippets, and correlate with users close to taking action.
- They cluster around the two features that differentiate VibeCV from generic resume builders: the **ATS checker** (keywords 1, 2, 4, 8) and **AI writing** (6), plus underserved **audience segments** (freshers, students, career changers, mobile-only users) that have low keyword competition but high install intent.
- Each guide targets a question format that Google's AI Overviews, ChatGPT, Perplexity, and Claude prefer to cite verbatim — directly supporting AI-assistant discoverability (see `llms.txt`).

## On-Page SEO Placement Plan

- **Title tags**: primary keyword within the first 60 characters, brand name last.
- **H1**: one per page, contains the primary/long-tail keyword naturally.
- **Meta description**: ~150–155 characters, includes keyword + a benefit + a CTA verb ("Download," "Try," "Build").
- **URL slugs**: keyword-matched, hyphenated, no stop-word stuffing.
- **Image alt text**: descriptive + keyword-adjacent (e.g., "VibeCV ATS resume checker showing 92% match score").
- **Internal linking**: every guide links back to the homepage download CTA and to 2–3 related guides; homepage FAQ links out to guides ("Learn More").
- **Structured data**: `SoftwareApplication` + `Organization` on homepage, `FAQPage` on homepage + every guide, `BreadcrumbList` + `Article`/`HowTo` on every guide — increases eligibility for rich results and AI citation.
- **Core Web Vitals**: single Tailwind CDN + deferred non-critical JS, compressed images, no layout-shifting fonts.
