AIMS Tools Hub - how to use and extend this site
=======================================

OPEN IT: double-click index.html. No server or build step needed.

WHAT IS INSIDE
- 23 tools in 8 categories (see tools.html). Each tool has its own page in tools/ and its own script in js/tools/.
- Required AdSense pages: About, Contact, Privacy Policy, Terms of Service, Disclaimer.
- js/common.js holds the shared helpers. css/style.css holds all styling (colors are at the top).

BEFORE YOU APPLY FOR ADSENSE
1. Buy a domain and host the folder (Netlify, Cloudflare Pages, GitHub Pages or any web host).
2. Search all files for "yourdomain.com" and replace it with your real domain (every page, sitemap.xml, robots.txt).
3. Replace the contact email (contact@yourdomain.com) with a real one on your domain.
4. Make sure every page has real, original text. Do not copy text from other sites.
5. After approval: paste your AdSense script in the <head> of every page (look for the comment), replace the "Ad space" boxes with ad units, and put your line in ads.txt.

ADD A NEW TOOL
1. Copy _template-new-tool.html into the tools/ folder and rename it (example: tools/loan-calculator.html).
2. Copy js/tools/_template.js to js/tools/loan-calculator.js and write the tool logic. The name in AIMS.reg(...) must match data-tool="..." in the page. Fix the script path at the bottom of the page.
3. Add a card for it in tools.html (inside the right category), and on index.html if it is popular. Copy an existing card.
4. Add the page to sitemap.xml.
(Or just ask Claude to add the tool and it will do all of these steps.)

ADD A CATEGORY: copy a "cat-block" section in tools.html, a category card in index.html and a link in the footer of each page.

CHANGE COLORS: edit the values at the top of css/style.css (the :root block).
