MANNIX DIGITAL CARD
===================

1. EDIT YOUR INFO
   Open index.html, find the CARD = { ... } block near the bottom, and fill in:
   phone, linkedin, instagram, facebook, github, etc.
   Empty ("") fields are hidden automatically, on the page and in the saved contact.
   Photo: put photo.jpg in this folder and set  photo: "photo.jpg"

2. TEST LOCALLY
   python -m http.server 5190     (then open http://localhost:5190)

3. PUT IT ONLINE (free). Easiest: Netlify Drop
   - Go to https://app.netlify.com/drop
   - Drag this whole "card" folder onto the page
   - You get a link like https://something.netlify.app  (rename it in Site settings)
   Alternatives: Vercel, Cloudflare Pages, GitHub Pages.

4. WRITE THE LINK TO YOUR NFC CARD
   - Install "NFC Tools" (iOS / Android)
   - Write > Add a record > URL/URI > paste your link > Write
   - Hold the card to the back of your phone when it asks
   - Test by tapping it on another phone

5. OPTIONAL: make a QR code of the same link (qr-code-generator sites) and put it on the back
   of the card, for phones without NFC.

When you change your info later, just redeploy the page. The card itself never needs rewriting.
