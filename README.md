# LIBAS ATELIER

## Social Order Hub

The repository now includes `social-order.html`, a mobile-friendly landing page intended to be used as the single link from Instagram, Facebook, TikTok, YouTube, and other social profiles.

### Flow

1. Visitor opens the social link.
2. Visitor can open the full catalog or choose a design.
3. The visitor fills in the order form.
4. The page prepares a complete order message.
5. **Submit & Open WhatsApp** opens WhatsApp with the order addressed to the configured Libas Atelier business number.
6. **Call Libas Atelier** opens the device phone dialer with the configured business number.

### Important configuration

Open `social-order.html` and edit the `CONFIG` object near the bottom:

- `businessWhatsApp` — Libas Atelier WhatsApp number in international digits, without `+` or spaces.
- `businessPhone` — Libas Atelier phone number for the `tel:` action.
- `social.instagram` — real Instagram profile URL.
- `social.facebook` — real Facebook profile URL.
- `social.tiktok` — real TikTok profile URL.
- `social.youtube` — real YouTube profile URL.
- `designCode` — the design shown on this landing page.

The current values are placeholders and must be replaced before publishing for real customers.

## GitHub Pages

`.github/workflows/deploy-pages.yml` deploys the repository to GitHub Pages whenever `main` changes. In the repository's **Settings → Pages**, select **GitHub Actions** as the publishing source. GitHub will then publish the site and provide the live Pages URL.

The existing catalog builder workflow remains separate and continues to build the catalog artifact on demand.
