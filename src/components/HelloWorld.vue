<template>
  <div class="kabsa-page">
    <!-- HERO -->
    <v-parallax
      :height="$vuetify.breakpoint.smAndDown ? 340 : 520"
      src="../assets/IMG_7735.png"
      class="kabsa-hero"
    >
      <div class="kabsa-hero-scrim"></div>
      <v-container class="kabsa-hero-inner">
        <v-row class="d-flex align-end" no-gutters>
          <v-col :cols="$vuetify.breakpoint.smAndDown ? 12 : 7">
            <h1 class="kabsa-title-main mt-16">Kabsa Spilled?</h1>
            <p class="kabsa-title-sub">Press Kit</p>
          </v-col>
          <v-col :cols="$vuetify.breakpoint.smAndDown ? 12 : 5" class="mt-4 mt-md-0">
            <div class="kabsa-hero-bio">
              <p class="kabsa-hero-bio-label">Game Bio</p>
              <p class="kabsa-hero-bio-text">
                you and your mate have to deliver the right amount of Kabsa Rice and Meat Pieces to the VIP customers of the Old themed Arabian restaurant, Each Garson on each side Balancing the Big, Hot and Weighted Kabsa Plate through the way.
              </p>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-parallax>

    <v-container class="kabsa-main">
      <!-- IDENTITY + ABOUT -->
      <v-row class="kabsa-main-grid" no-gutters>
        <!-- Identity / links card -->
        <v-col :cols="$vuetify.breakpoint.mdAndUp ? 3 : 12" class="kabsa-col-identity">
          <v-card flat class="kabsa-card kabsa-identity-card">
            <img
              src="../assets/Kabsa Spilled Game Logo.png"
              class="kabsa-medallion"
              alt="Kabsa Spilled logo"
            />
            <p class="kabsa-game-title">KABSA SPILLED?</p>
            <p class="kabsa-studio-credit">
              By
              <a href="https://store.steampowered.com/curator/45736123" target="_blank" rel="noopener">
                OliveRoots Studio
              </a>
            </p>

            <v-btn block class="kabsa-btn kabsa-btn-gold" @click="downloadAll">
              <v-icon class="mr-2" size="18">mdi-download</v-icon>
              Download images
            </v-btn>

            <v-divider class="kabsa-divider"></v-divider>

            <p class="kabsa-field-label">Platform</p>
            <v-btn
              block
              class="kabsa-btn kabsa-btn-platform"
              href="https://store.steampowered.com/app/4582550/Kabsa_Spilled/"
              target="_blank"
              rel="noopener"
            >
              <v-icon class="mr-2" size="18">fa-brands fa-steam</v-icon>
              Steam
            </v-btn>

            <v-divider class="kabsa-divider"></v-divider>

            <p class="kabsa-field-label">Follow</p>
            <div class="kabsa-social-grid">
              <v-btn class="kabsa-chip kabsa-chip--youtube" href="https://www.youtube.com/@oliverootsdev/featured" target="_blank" rel="noopener">
                <v-icon size="16" class="mr-1">fa-brands fa-youtube</v-icon> YouTube
              </v-btn>
              <v-btn class="kabsa-chip kabsa-chip--twitter" href="https://x.com/OliverootsStd?t=0rvTzcNTiaGBf-mwiIPPEw&s=09" target="_blank" rel="noopener">
                <v-icon size="16" class="mr-1">fa-brands fa-x-twitter</v-icon> Twitter/X
              </v-btn>
              <v-btn class="kabsa-chip kabsa-chip--tiktok" href="https://www.tiktok.com/@kabsaspilled0?_r=1" target="_blank" rel="noopener">
                <v-icon size="16" class="mr-1">fa-brands fa-tiktok</v-icon> TikTok
              </v-btn>
              <v-btn class="kabsa-chip kabsa-chip--discord" href="https://discord.gg/5GGWHwhy" target="_blank" rel="noopener">
                <v-icon size="16" class="mr-1">fa-brands fa-discord</v-icon> Discord
              </v-btn>
            </div>

            <div class="kabsa-release-row">
              <p class="kabsa-field-label">Demo release date</p>
              <p class="kabsa-release-value">Steam · 1st Sep 2026</p>
            </div>
          </v-card>
        </v-col>

        <!-- About / features card -->
        <v-col :cols="$vuetify.breakpoint.mdAndUp ? 7 : 12" class="kabsa-col-content">
          <v-card flat class="kabsa-card kabsa-content-card">
            <h2 class="kabsa-section-heading">About This Game</h2>
            <div class="kabsa-rule"></div>
            <p class="kabsa-body-text">
              Grab a buddy and lead the adventure of two chefs through deadly firepits, tricky platforms, angry vendors and much worse things to DEFENITELY make your friendship better
            </p>

            <div class="kabsa-section-block">
              <h2 class="kabsa-section-heading">Game Features</h2>
              <div class="kabsa-rule"></div>
              <ul class="kabsa-features">
                <li>Realistic Plate Balancing and Physics.</li>
                <li>Singleplayer, Couch-Party &amp; Online Co-op modes.</li>
                <li>Gameplay Timer and Death Counter for speedrunner heroes.</li>
                <li>Arabic Themed Old Places Vibe.</li>
                <li>So much fun and pain in one place.</li>
              </ul>
            </div>
          </v-card>
        </v-col>
      </v-row>

      <!-- MEDIA -->
      <div class="kabsa-section-block">
        <h2 class="kabsa-section-heading">Media</h2>
        <div class="kabsa-rule"></div>
        <p class="kabsa-media-note">
          <span class="kabsa-bold">Trailer |</span>
          Official Demo Trailer on
          <a href="https://www.youtube.com/watch?v=Kr5j7oiXnxk" target="_blank" rel="noopener">Youtube</a>
        </p>

        <div class="kabsa-frame">
          <v-responsive :aspect-ratio="16 / 9" class="kabsa-frame-inner">
            <iframe
              width="100%"
              height="100%"
              src="https://www.youtube.com/embed/Kr5j7oiXnxk"
              title="Kabsa Spilled? - Official Demo Trailer"
              frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              allowfullscreen
            ></iframe>
          </v-responsive>
        </div>
      </div>

      <!-- SCREENSHOTS -->
      <div class="kabsa-section-block">
        <div class="kabsa-shots-head">
          <div>
            <h2 class="kabsa-section-heading">Screenshots</h2>
            <div class="kabsa-rule"></div>
          </div>
          <v-btn class="kabsa-btn kabsa-btn-outline" @click="downloadAll">
            <v-icon class="mr-2" size="18">mdi-download</v-icon>
            Download images
          </v-btn>
        </div>

        <div class="kabsa-frame">
          <v-carousel
            hide-delimiter-background
            :height="$vuetify.breakpoint.smAndDown ? 280 : 480"
            class="kabsa-carousel"
          >
            <v-carousel-item v-for="(screenshot, i) in screenshots" :key="i">
              <v-img :src="screenshot" contain></v-img>
            </v-carousel-item>
          </v-carousel>
        </div>
      </div>

      <footer class="kabsa-footer">
        <div class="kabsa-footer-rule"></div>
        <p class="kabsa-footer-text">Copyrights © 2025 OliveRoots | All Rights Reserved</p>
      </footer>
    </v-container>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  methods: {
    async downloadAll () {
      const link = document.createElement('a')
      link.href = 'https://oliveroots.github.io/kabsa-spilled/Game Images/Game Images.zip'
      link.download = 'Game Images.zip'
      link.click()
    }
  },
  data: () => ({
    // Not currently wired to the template. Kept as a starting point if you
    // add an in-page nav later (see suggestion in chat).
    sideButtons: [
      { text: 'Links', to: 'mdi-clock' },
      { text: 'Description', to: 'mdi-account' },
      { text: 'Features', to: 'mdi-account' },
      { text: 'Media', to: 'mdi-account' },
      { text: 'Screenshots', to: 'mdi-account' },
      { text: 'About Developer', to: 'mdi-flag' }
    ],
    screenshots: [
      require('@/assets/Game Images/screen1.png'),
      require('@/assets/Game Images/screen2.png'),
      require('@/assets/Game Images/screen3.png'),
      require('@/assets/Game Images/screen4.png'),
      require('@/assets/Game Images/screen5.png'),
      require('@/assets/Game Images/screen6.png'),
      require('@/assets/Game Images/screen7.png'),
      require('@/assets/Game Images/screen8.png')
    ]
  })
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lalezar&family=Cairo:wght@300;400;500;600;700;800&display=swap');

/* ---------- Design tokens ---------- */
.kabsa-page {
  --kabsa-ink: #2a1810;
  --kabsa-ink-70: rgba(42, 24, 16, 0.72);
  --kabsa-ink-50: rgba(42, 24, 16, 0.5);
  --kabsa-ink-12: rgba(42, 24, 16, 0.12);
  --kabsa-ink-06: rgba(42, 24, 16, 0.06);
  --kabsa-cream: #fbf1de;
  --kabsa-cream-deep: #f3e2be;
  --kabsa-surface: #fffdf8;
  --kabsa-gold: #e8a72c;
  --kabsa-gold-deep: #c6841a;
  --kabsa-gold-tint: rgba(232, 167, 44, 0.14);
  --kabsa-paprika: #b23a22;
  --kabsa-navy: #16233a;
  --kabsa-radius-lg: 26px;
  --kabsa-radius-md: 16px;
  --kabsa-radius-pill: 999px;
  --kabsa-shadow: 0 18px 44px -16px rgba(42, 24, 16, 0.32);

  background: var(--kabsa-cream);
  color: var(--kabsa-ink);
  font-family: 'Cairo', sans-serif;
}

/* ---------- Hero ---------- */
.kabsa-hero .v-parallax__content {
  display: flex;
  align-items: flex-end;
  padding: 0;
}
.kabsa-hero-scrim {
  position: absolute;
  inset: 0;
  background: linear-gradient(0deg, rgba(18, 10, 6, 0.82) 0%, rgba(18, 10, 6, 0.35) 45%, rgba(18, 10, 6, 0) 75%);
  z-index: 1;
}
.kabsa-hero-inner {
  position: relative;
  z-index: 2;
  width: 100%;
  padding-bottom: 40px;
}
.kabsa-title-main {
  font-family: 'Lalezar', sans-serif;
  font-weight: 400;
  font-size: clamp(2.4rem, 5.2vw, 4.2rem);
  line-height: 1;
  color: #fbf1de;
  text-shadow: 0 6px 24px rgba(0, 0, 0, 0.35);
  margin: 0;
}
.kabsa-title-sub {
  margin: 10px 0 0;
  font-weight: 500;
  color: var(--kabsa-gold);
  font-size: 1.05rem;
}
.kabsa-hero-bio {
  background: rgba(20, 11, 7, 0.45);
  border: 1px solid rgba(255, 255, 255, 0.14);
  backdrop-filter: blur(8px);
  border-radius: var(--kabsa-radius-md);
  padding: 18px 22px;
  max-width: 440px;
}
.kabsa-hero-bio-label {
  font-weight: 700;
  color: var(--kabsa-gold);
  margin: 0 0 8px;
  font-size: 0.95rem;
}
.kabsa-hero-bio-text {
  margin: 0;
  color: rgba(251, 241, 222, 0.92);
  font-size: 0.95rem;
  line-height: 1.65;
}

/* ---------- Main layout ---------- */
.kabsa-main {
  margin-top: -56px;
  position: relative;
  z-index: 2;
  max-width: 1180px;
}
.kabsa-main-grid {
  margin: 0 -14px;
  justify-content: space-around;
}
.kabsa-col-identity,
.kabsa-col-content {
  padding: 14px;
}
.kabsa-card {
  background: var(--kabsa-surface) !important;
  border: 1px solid var(--kabsa-ink-06);
  border-radius: var(--kabsa-radius-lg) !important;
  box-shadow: var(--kabsa-shadow) !important;
  height: 100%;
}

/* Identity card */
.kabsa-identity-card {
  padding: 32px 26px;
  text-align: center;
}
.kabsa-medallion {
  width: 128px;
  height: 128px;
  border-radius: 50%;
  object-fit: cover;
  border: 3px solid var(--kabsa-gold);
  box-shadow: 0 0 0 5px var(--kabsa-cream-deep);
  margin-bottom: 16px;
}
.kabsa-game-title {
  font-weight: 800;
  font-size: 1.35rem;
  margin: 0 0 4px;
}
.kabsa-studio-credit {
  font-size: 0.92rem;
  color: var(--kabsa-ink-70);
  margin: 0 0 18px;
}
.kabsa-studio-credit a {
  color: var(--kabsa-paprika);
  font-weight: 600;
  text-decoration: none;
}
.kabsa-studio-credit a:hover {
  text-decoration: underline;
}
.kabsa-divider {
  margin: 22px 0 !important;
  border-color: var(--kabsa-ink-12) !important;
}
.kabsa-field-label {
  font-size: 0.82rem;
  font-weight: 600;
  color: var(--kabsa-ink-50);
  text-align: left;
  margin: 0 0 10px;
}
.kabsa-social-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px;
}
.kabsa-release-row {
  margin-top: 22px;
  text-align: left;
}
.kabsa-release-value {
  font-size: 0.92rem;
  font-weight: 600;
  margin: 0;
}

/* Buttons — override Vuetify defaults, styled via classes instead of the
   `color` prop so nothing fights us via inline styles */
.kabsa-btn.v-btn {
  text-transform: none !important;
  font-family: 'Cairo', sans-serif !important;
  font-weight: 600 !important;
  letter-spacing: normal !important;
  border-radius: var(--kabsa-radius-pill) !important;
  box-shadow: none !important;
  height: auto !important;
  padding: 11px 20px !important;
  transition: transform 0.16s ease, box-shadow 0.16s ease, background-color 0.16s ease;
}
.kabsa-btn.v-btn:hover {
  transform: translateY(-2px);
}
.kabsa-btn-gold.v-btn {
  background-color: var(--kabsa-gold) !important;
  color: var(--kabsa-ink) !important;
}
.kabsa-btn-gold.v-btn:hover {
  background-color: var(--kabsa-gold-deep) !important;
  box-shadow: 0 10px 20px -8px rgba(198, 132, 26, 0.55) !important;
}
.kabsa-btn-platform.v-btn {
  background-color: var(--kabsa-navy) !important;
  color: #fff !important;
  margin-top: 16px !important;
}
.kabsa-btn-platform.v-btn:hover {
  box-shadow: 0 10px 20px -8px rgba(22, 35, 58, 0.5) !important;
}
.kabsa-btn-outline.v-btn {
  background-color: transparent !important;
  border: 1.5px solid var(--kabsa-gold) !important;
  color: var(--kabsa-gold-deep) !important;
}
.kabsa-btn-outline.v-btn:hover {
  background-color: var(--kabsa-gold-tint) !important;
}

/* Social chips */
.kabsa-chip.v-btn {
  text-transform: none !important;
  font-family: 'Cairo', sans-serif !important;
  font-weight: 600 !important;
  font-size: 0.85rem !important;
  background-color: var(--kabsa-cream) !important;
  border: 1px solid var(--kabsa-ink-12) !important;
  color: var(--kabsa-ink) !important;
  border-radius: var(--kabsa-radius-pill) !important;
  box-shadow: none !important;
  height: auto !important;
  padding: 9px 10px !important;
  min-width: 0 !important;
  transition: background-color 0.16s ease, transform 0.16s ease;
}
.kabsa-chip.v-btn:hover {
  transform: translateY(-1px);
  background-color: var(--kabsa-gold-tint) !important;
}
.kabsa-chip--youtube .v-icon { color: #e0332e !important; }
.kabsa-chip--twitter .v-icon { color: #13171a !important; }
.kabsa-chip--tiktok .v-icon { color: #ef2a63 !important; }
.kabsa-chip--discord .v-icon { color: #5865f2 !important; }

/* Content card */
.kabsa-content-card {
  padding: 34px 36px;
}
.kabsa-section-heading {
  font-size: 1.5rem;
  font-weight: 800;
  margin: 0 0 8px;
}
.kabsa-rule {
  width: 44px;
  height: 4px;
  background: var(--kabsa-gold);
  border-radius: 2px;
  margin: 0 0 16px;
}
.kabsa-body-text {
  font-size: 0.98rem;
  line-height: 1.75;
  color: var(--kabsa-ink-70);
  max-width: 64ch;
  margin: 0;
}
.kabsa-features {
  list-style: none;
  margin: 22px 0 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  gap: 10px;
  max-width: 60ch;
}
.kabsa-features li {
  font-size: 0.96rem;
  line-height: 1.6;
  color: var(--kabsa-ink-70);
  padding-left: 20px;
  position: relative;
}
.kabsa-features li::before {
  content: '—';
  color: var(--kabsa-gold-deep);
  font-weight: 700;
  position: absolute;
  left: 0;
}

.kabsa-section-block {
  margin-top: 34px;
}
.kabsa-media-note {
  font-size: 0.9rem;
  color: var(--kabsa-ink-50);
  margin: 0 0 16px;
}
.kabsa-media-note a {
  color: var(--kabsa-paprika);
  font-weight: 600;
  text-decoration: none;
}
.kabsa-bold {
  font-weight: 700;
  color: var(--kabsa-ink);
}

/* Framed media / carousel */
.kabsa-frame {
  background: var(--kabsa-surface);
  border: 1px solid var(--kabsa-ink-12);
  border-radius: var(--kabsa-radius-lg);
  padding: 10px;
  box-shadow: var(--kabsa-shadow);
}
.kabsa-frame-inner {
  border-radius: 14px !important;
  overflow: hidden;
  border: 1px solid var(--kabsa-ink-06);
}
.kabsa-carousel {
  border-radius: 14px !important;
  overflow: hidden;
}
.kabsa-shots-head {
  display: flex;
  align-items: flex-end;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 12px;
  margin-bottom: 16px;
}
.kabsa-shots-head .kabsa-section-heading,
.kabsa-shots-head .kabsa-rule {
  margin-bottom: 0;
}
.kabsa-shots-head .kabsa-rule {
  margin-top: 8px;
}

/* Footer */
.kabsa-footer {
  margin-top: 56px;
  padding: 26px 0 20px;
}
.kabsa-footer-rule {
  height: 1px;
  background: linear-gradient(90deg, transparent, var(--kabsa-gold), transparent);
  margin-bottom: 20px;
}
.kabsa-footer-text {
  text-align: center;
  font-size: 0.85rem;
  color: var(--kabsa-ink-50);
  margin: 0;
}
.v-card > *:first-child:not(.v-btn):not(.v-chip):not(.v-avatar), .v-card > .v-card__progress + *:not(.v-btn):not(.v-chip):not(.v-avatar){
      border-top-left-radius: 50%;
    border-top-right-radius: 50%;
}
@media (max-width: 600px) {
  .kabsa-content-card,
  .kabsa-identity-card {
    padding: 26px 20px;
  }
  .kabsa-main {
    margin-top: -36px;
  }
}
</style>
