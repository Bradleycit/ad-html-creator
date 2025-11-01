# ad-html-creator

Amazon Interstitial Ad Generator
Create beautiful, mobile-friendly Amazon affiliate ads with live preview — no more "Fetching image..." delays!
Failed to load imageView link

Features

Live HTML Preview – See exactly how your ad will look before copying
Auto Image Fetching – Pulls the largest product image directly from Amazon (with 3s timeout)
Manual Image Override – Paste any image URL if needed
Smart Price Formatting – Show sale price with strikethrough original
Affiliate Link Builder – Automatically adds your tag + ref=yourls
One-Click Copy – Copy clean, minified HTML ready for YOURLS or any site
Mobile-Responsive Design – Looks great on all devices
No Backend Required – 100% client-side, works offline


How to Use

Open index.html in any modern browser (Chrome, Firefox, Safari, etc.)
Paste your Amazon product URL
(Optional) Add:

Custom image URL
Your affiliate tag
Ad title, sale price, original price


Click "Generate Ad + Preview"
See the live preview instantly
Click "Copy HTML" and paste into YOURLS, WordPress, or any HTML editor


Pro Tip: Right-click the product image on Amazon → Copy image address → paste into the Product Image URL field for fastest results.


Example Output
html<div style="background:#fff;padding:25px;border-radius:15px;text-align:center;box-shadow:0 4px 15px rgba(0,0,0,0.1);max-width:100%;">
  <img src="https://m.media-amazon.com/images/I/71j3Z3Z3Z3L._AC_SL1500_.jpg" alt="Product" style="max-width:100%;height:auto;border-radius:10px;margin-bottom:15px;">
  <h3 style="margin:8px 0;font-size:20px;color:#232f3e;">Limited Time Deal!</h3>
  <p style="margin:8px 0;color:#B12704;font-weight:bold;font-size:18px;"><del>$299.99</del> $199.99</p>
  <a href="https://www.amazon.com/dp/B0FFPZRPX9?tag=yourtag-20&ref=yourls" target="_blank" style="background:#ff9900;color:#fff;text-decoration:none;padding:12px 28px;border-radius:50px;font-weight:bold;font-size:17px;display:inline-block;">
    View Deal on Amazon
  </a>
  <p style="margin-top:12px;font-size:11px;color:#666;">
    Affiliate link • As an Amazon Associate we earn from qualifying purchases
  </p>
</div>

Tech Stack

HTML5
CSS3 (Flexbox, responsive design)
Vanilla JavaScript (ES6+)
allorigins.win proxy for CORS-free Amazon scraping
No dependencies, no build tools


Local Development
Just open index.html — no server needed!
bash# Clone the repo
git clone https://github.com/yourusername/amazon-ad-generator.git

# Open in browser
open index.html

Customization
Want to tweak the design?
Edit the inline styles in the <script> section of index.html:
js// Change button color
background:#ff9900;  →  background:#ff5733;

// Change font sizes, padding, border radius, etc.
All styles are inline for maximum compatibility with email & embed platforms.

Compliance & Best Practices

Includes required "As an Amazon Associate..." disclosure
Uses target="_blank" for external links
ref=yourls parameter for tracking in YOURLS
Fully compliant with Amazon Associates Program policies


FAQ
Why use a proxy (allorigins.win)?
Amazon blocks direct cross-origin requests. The proxy fetches the page safely.
What if the image doesn't load?

Falls back to a clean placeholder: No Image
Or use manual image URL for guaranteed control

Can I use this commercially?
Yes! 100% free for personal and commercial use.

Contributing
Pull requests welcome! Especially:

Better image detection regex
Support for international Amazon domains
Dark mode toggle
Export to PNG feature


License
MIT License – Free to use, modify, and distribute.

Built with ❤️ for affiliate marketers who hate broken previews.

⭐ Star this repo if it saved you time!
🐛 Found a bug? Open an issue
Made by [Your Name] – Amazon Affiliate Tools