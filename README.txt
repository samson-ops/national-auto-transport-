NATIONAL AUTO TRANSPORT — WEBSITE PACKAGE
=========================================

CONTENTS
  index.html            Homepage                  URL: /
  how-it-works/         Shipping process page     URL: /how-it-works/
  services/             All 9 services in detail  URL: /services/
  reviews/              Customer reviews          URL: /reviews/
  faq/                  Full FAQ                  URL: /faq/
  locations/            Office directory          URL: /locations/
  sitemap.xml           All 31 URLs for Google Search Console
  robots.txt            Allows crawling, points to the sitemap
  city/                 25 city pages, one folder each, e.g.
                        city/auto-transport-birmingham-alabama/index.html
                        (URL: /city/auto-transport-birmingham-alabama/)
  css/                  styles.css (shared) and pages.css (interior pages)
  images/               All site images, named by where they're used

SITE STRUCTURE / URLS
  City pages live at clean directory URLs, e.g.:
    https://nationalautoship.com/city/auto-transport-birmingham-alabama/
  Each is a folder under /city/ containing an index.html, so the clean
  URL works automatically on any standard host (Apache, Nginx, Netlify,
  Vercel, cPanel). City pages use root-relative paths (/css/, /images/)
  and include a canonical tag pointing at nationalautoship.com.

HOW TO USE
  1. Preview: because of the root-relative paths, preview with a local
     server rather than double-clicking files. Easiest way:
       cd into this folder, run:  python3 -m http.server 8000
       then open http://localhost:8000
     (Or just upload to your host — see below.)
  2. Deploy: upload EVERYTHING in this folder together (index.html, all page folders, city/, css/, images/, sitemap.xml, robots.txt), at the ROOT of the domain (the pretty /city/ URLs and root-relative paths require the site to live at nationalautoship.com's root, not in a subfolder) to any
     web host (Netlify, Vercel, cPanel, GoDaddy, Hostinger, etc.).
     Keep the folder structure exactly as-is.

COMPATIBILITY
  Tested-for targets: iOS Safari, Android Chrome/Samsung Internet,
  desktop Chrome, Edge, Firefox, Safari, and Opera. The site is plain
  HTML/CSS/vanilla JS (no frameworks), which is the most compatible
  stack there is. Mobile specifics: 16px inputs (no iOS zoom-on-focus),
  safe-area padding for notched iPhones, 44px+ tap targets, scrollable
  tables, and layouts tested down to 320px-wide screens.

PHONE NUMBERS
  Main number (866) 459-6389 appears on the homepage and all non-city
  pages. Each city page uses its own local office number throughout.

BEFORE GOING LIVE — REPLACE THESE PLACEHOLDERS
  - Email:         quotes@nationalautotransport.com
  - Reviews:       sample names/text — swap for real customer reviews
  - Rates table:   sample price ranges — adjust to your actual pricing
                   (homepage AND each city page's route table)

CITY PAGES
  Each city page uses its own local phone number in the top bar, header,
  mobile call bar, and CTAs. The addresses you provided are shown with a
  Google Maps embed. Route prices and "also serving" city lists are
  editable placeholders — adjust to your real data.

QUOTE FORM
  The homepage quote section (#quote) is the Berocker booking widget
  (widget.berocker.com) connected to your Ship Guy account via the
  api_key in the iframe src. All "Get a Quote" buttons across the site
  scroll/link to it. If the widget is taller or shorter than expected,
  adjust the iframe height attribute in index.html.
