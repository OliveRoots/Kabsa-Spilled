<template>
  <div>
    <v-parallax
      :height="$vuetify.breakpoint.smAndDown ? 300 : 500"
      src="../assets/image_2025-08-23_05-58-13-1920x1080.png"
    >
      <v-row class="d-flex justify-center align-center">
        <v-col :cols="$vuetify.breakpoint.smAndDown ? 12 : 6">
          <p class="arabic-bold ml-2 title-text">Blind Memory Press Kit</p>
        </v-col>
        <v-col :cols="$vuetify.breakpoint.smAndDown ? 12 : 6">
          <p class="arabic-bold subtitle-text mb-3">Game Bio</p>
          <p class="arabic mb-5">
            Dive into a haunting mystery where you wake up half-blind and amnesiac, trapped in a time-looping nightmare. Uncover the truth through shifting 3D and 2D perspectives, where every revelation twists reality further.
          </p>
        </v-col>
      </v-row>
    </v-parallax>

    <v-container>
      <v-row class="d-flex flex-wrap align-start justify-center">
        <!-- Image Column -->
        <v-col
          :cols="$vuetify.breakpoint.smAndDown ? 12 : 3"
           :class="{'first-col': $vuetify.breakpoint.mdAndUp}"
          class="d-flex flex-column align-start "
        >
          <img
            src="../assets/Vertical Capsule 748px x 896px.png"
            width="100%"
            class="rounded-xl"
            style="border: 2px solid #265F67;"
            alt=""
          />
          <p class="arabic-bold ma-2 game-title">BLIND MEMORY</p>
          <p class="arabic-bold mx-2">
            BY
            <a href="https://store.steampowered.com/curator/45736123" target="_blank" style="text-decoration: none;">
              OliveRoots Studio
            </a>
          </p>
          <v-btn color="#29ABC5" class="rounded-xl arabic white--text ml-2" @click="downloadAll">
            <v-icon class="mx-2">mdi-download</v-icon>
            Download Images
          </v-btn>
        </v-col>

        <!-- Links Column -->
        <v-col :cols="$vuetify.breakpoint.smAndDown ? 12 : 2" class="mr-5">
          <p class="arabic-bold ma-2 links-title">Links</p>
          <p class="arabic-bold ma-2">Platform:</p>
          <v-btn color="#1b2838" class="rounded-xl arabic white--text ma-2" href="https://store.steampowered.com/app/3894660/Blind_Memory/" target="_blank">
            <v-icon class="mx-2">fa-brands fa-steam</v-icon> Steam
          </v-btn>

          <p class="arabic-bold ma-2">Social Media:</p>
          <v-btn color="#ff0000" rounded="xl" class="rounded-xl arabic white--text ma-2" href="https://www.youtube.com/@studiooliveroots/featured" target="_blank">
            <v-icon class="mx-2">fa-brands fa-youtube</v-icon> Youtube
          </v-btn>
          <v-btn color="#13171A" rounded="xl" class="rounded-xl arabic white--text ma-2" href="https://x.com/OliverootsStd?t=0rvTzcNTiaGBf-mwiIPPEw&s=09" target="_blank">
            <v-icon class="mx-2">fa-brands fa-x-twitter</v-icon> Twitter/X
          </v-btn>
          <v-btn color="#7289DA" rounded="xl" class="rounded-xl arabic white--text ma-2" href="https://discord.gg/5GGWHwhy" target="_blank">
            <v-icon class="mx-2">fa-brands fa-discord</v-icon> Discord
          </v-btn>

          <p class="arabic-bold ma-2">Demo Release Date:</p>
          <p class="arabic ma-2">Steam | 13 October 2025</p>
        </v-col>

        <!-- About Column -->
        <v-col :cols="$vuetify.breakpoint.smAndDown ? 12 : 6" class="ml-16">
          <p class="arabic-bold subtitle-text mb-3">About This Game</p>
          <p class="arabic mb-5">
            Blind Memory is an affluent experience to feel Lost, Chaos, and Blinded...
          </p>

          <p class="arabic-bold subtitle-text mb-3">Game Features</p>
          <ul>
            <li class="arabic mb-1">Dual-Perspective Gameplay – Mix of 3D exploration + 2D scenes</li>
            <li class="arabic mb-1">Amnesia + Time Loops – unraveling mysteries</li>
            <li class="arabic mb-1">Atmospheric Horror – Focus on sound design & visual</li>
            <li class="arabic mb-1">Narrative Twists – mind-bending experience where nothing is as it seems.</li>
          </ul>
        </v-col>
      </v-row>

      <!-- Media & Screenshots -->
      <v-row class="d-flex flex-column align-start justify-center">
        <v-col cols="12">
          <p class="arabic-bold ma-2 media-title">Media</p>
          <p class="arabic ma-2">
            <span class="arabic-bold">Trailer |</span>
            Official Alpha Gameplay Trailer on
            <a href="https://www.youtube.com/watch?v=0Q4JvyuMB1w" target="_blank">Youtube</a>
          </p>

          <v-responsive class="rounded-xl" :aspect-ratio="$vuetify.breakpoint.smAndDown ? 16/9 : 16/9" style="height: auto;">
            <iframe
              width="100%"
              height="100%"
              src="https://www.youtube.com/embed/0Q4JvyuMB1w"
              title="Blind Memory - Official Alpha Gameplay Trailer"
              frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              allowfullscreen
            ></iframe>
          </v-responsive>
        </v-col>

        <v-col cols="12">
          <p class="arabic-bold ma-2 media-title">Screenshots</p>
          <v-btn color="#29ABC5" class="rounded-xl arabic white--text ma-2" @click="downloadAll">
            <v-icon class="mx-2">mdi-download</v-icon> Download Images
          </v-btn>

          <v-carousel hide-delimiter-background :height="$vuetify.breakpoint.smAndDown ? 300 : 600" class="rounded-xl">
            <v-carousel-item v-for="(screenshot, i) in screenshots" :key="i">
              <v-img :src="screenshot" contain class="rounded-lg"></v-img>
            </v-carousel-item>
          </v-carousel>
        </v-col>
      </v-row>

      <v-divider class="ma-4"></v-divider>
      <v-footer padless variant="absolute" color="transparent">
        <v-col class="text-center" cols="12">
          <p class="arabic mx-16 text-center" style="font-size: small;">
            Copyrights © 2025 OliveRoots | All Rights Reserved
          </p>
        </v-col>
      </v-footer>
    </v-container>
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  methods: {
    async downloadAll () {
      const link = document.createElement('a')
      link.href = 'https://oliveroots.github.io/Blind-memory/Game Images/Game Images.zip'
      link.download = 'Game Images.zip'
      link.click()
    }

  },
  data: () => ({
    sideButtons: [
      { text: 'Links', to: 'mdi-clock' },
      { text: 'Description', to: 'mdi-account' },
      { text: 'Features', to: 'mdi-account' },
      { text: 'Media', to: 'mdi-account' },
      { text: 'Screenshots', to: 'mdi-account' },
      { text: 'About Developer', to: 'mdi-flag' }
    ],
    screenshots: [
      require('@/assets/Game Images/screen1.jpg'),
      require('@/assets/Game Images/screen2.jpg'),
      require('@/assets/Game Images/screen3.jpg'),
      require('@/assets/Game Images/screen4.jpg'),
      require('@/assets/Game Images/screen5.png'),
      require('@/assets/Game Images/screen6.png')
    ]
  })
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,100..900;1,100..900&display=swap');
.first-col {
  margin-top: -150px; /* adjust value as you like */
  z-index: 2;
}
.arabic-bold{
  font-family: "Roboto", sans-serif !important;
  font-weight: 700 !important;
  line-height: inherit !important;
}
.arabic{
  font-family: "Roboto", sans-serif !important;
  font-weight: 400;
  line-height: inherit !important;
}

/* Responsive font sizes */
.title-text {
  font-size: 3.2rem;
}
.subtitle-text {
  font-size: 1.5rem;
}
.game-title {
  font-size: 2rem;
}
.links-title,
.media-title {
  font-size: 2rem;
}

@media (max-width: 600px) {
  .first-col {
    margin-top: -50px;
  }
  .title-text {
    font-size: 2rem !important;
  }
  .subtitle-text {
    font-size: 1.2rem !important;
  }
  .game-title {
    font-size: 1.5rem !important;
  }
  .links-title,
  .media-title {
    font-size: 1.5rem !important;
  }
}
</style>
