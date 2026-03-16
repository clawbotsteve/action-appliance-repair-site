# Analytics Setup (GA4 + GTM + Search Console)

## 1) Google Tag Manager
1. Create a GTM container for `actionappliancerepairphoenix.com`.
2. Replace `GTM-XXXXXXX` in your deployment snippets.
3. Publish container version 1.

## 2) Google Analytics 4
1. Create a GA4 property.
2. Get Measurement ID (`G-XXXXXXXXXX`).
3. Add GA4 Configuration tag in GTM with that ID.
4. Trigger on All Pages.

## 3) Events to verify (already wired in site)
- `book_click`
- `call_click`
- `form_submit`
- `booking_submitted`

Check in:
- GTM Preview mode
- GA4 Realtime view

## 4) Search Console
1. Add property for `https://actionappliancerepairphoenix.com`.
2. Verify by DNS (recommended).
3. Submit sitemap:
   - `https://actionappliancerepairphoenix.com/sitemap.xml`

## 5) Quick QA
- Visit Home, Booking, Contact pages.
- Click Book button once.
- Click phone link once.
- Submit contact form once.
- Confirm events in GA4 Realtime and GTM Preview.
