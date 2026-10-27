# AXNT Wood Products landing page

A one-page site for AXNT Wood Products, a custom door, molding, and millwork shop in Logan, Utah. Its only job is to turn builders, contractors, and homeowners into quote requests and phone calls. It is plain static HTML with no build step: all copy, CSS, and JS live in `index.html` (Google Fonts is the only outside dependency), the quote form runs on Netlify Forms, and `thanks.html` is the page people land on after submitting. To edit copy, open `index.html`, change the text between the tags, commit, and push to `main`; Netlify redeploys automatically in under a minute. To add a photo, put the file in an `img/` folder and replace the matching `<div class="ph-box">` placeholder with the `<img>` tag shown in the comment at the top of `index.html`.

## Still needed from the owner

Items marked `[confirm]` on the page:

1. Doors: interior **and** exterior, or interior only?
2. Moldings: are custom molder knives made in-house?
3. Delivery: do you deliver, or is it shop pickup only?
4. Reply time: is "within 1 business day" accurate? (also on `thanks.html`)
5. Service radius: "Logan, Cache Valley, and northern Utah" correct?
6. Shop hours (currently `[Mon–Fri hours]`).

Placeholders:

7. Logo file (the header wordmark is text for now).
8. Eight photos: hero, Custom Doors, Moldings, Millwork, Shop Drawings, two shop-floor shots, plus a 1200 × 630 social share image. Sizes are printed on each placeholder.
9. Social proof: Google rating, three real customer quotes (with permission), client logos. **If these aren't available, delete the whole "Trusted by Cache Valley builders" section** instead of launching with placeholders.
10. Facebook page URL (footer link is `#`).
11. Form notifications: submissions currently email hogan@tearawaymedia.com (Netlify > Site configuration > Notifications). Switch or add rex@axntwp.com when the site goes live.
12. Custom domain: once connected, update the `canonical`, `og:url`, and JSON-LD `url` in `index.html`.

## Form notes

- Netlify Forms caps a submission (including the uploaded file) at 8 MB; the page blocks bigger files and tells people to email them instead.
- Spam: Netlify's honeypot field `bot-field` is wired in.
