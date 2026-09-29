# Instagram Reels: manual gallery updates

The gallery is updated manually. It does not require an Instagram API key or account access. The current five Reels are listed in `assets/instagram-reels.js`; four use their matching local repair cover images.

## Add or replace a Reel

1. Add its cover image under `assets/instagram/` (WebP, JPG, or PNG).
2. Edit `assets/instagram-reels.js` and add one object to `window.BULVAR_INSTAGRAM_REELS`:

   ```js
   {
     title: '15 Pro Max ekran değişimi',
     permalink: 'https://www.instagram.com/reel/REEL_SHORTCODE/',
     thumbnailUrl: 'assets/instagram/15-pro-max-ekran-degisimi.webp'
   }
   ```

3. Keep the six newest Reels in the array. The cards use the supplied cover and title; clicking a card opens the Reel in the site's video viewer.
4. Upload the changed files with the rest of the site when the next planned GitHub update is approved.

If a Reel cover is not available yet, its card keeps the title and Instagram link and shows a branded cover placeholder until an image is added. When the list is empty, the original local repair cards remain as a fallback.
