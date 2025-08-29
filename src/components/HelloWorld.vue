<template>
  <div>
      <v-parallax
    height="500"
    src="../assets/image_2025-08-23_05-58-13-1920x1080.png"
  >
  <v-row class="d-flex flex-row justify-center align-center">
    <v-col cols="6">
       <p class="arabic-bold ml-10" style="font-size: 3.2rem;">Blind Memory Press Kit</p>
      </v-col>
    <v-col>
                  <p class="arabic-bold mb-3" style="font-size: 1.5rem;"> Game Bio </p>
            <p class="arabic mb-5">Dive into a haunting mystery where you wake up half-blind and amnesiac, trapped in a time-looping nightmare. Uncover the truth through shifting 3D and 2D perspectives, where every revelation twists reality further.</p>
    </v-col>
  </v-row>
</v-parallax>
    <v-container>
      <v-row class="d-flex flex-row align-start justify-center">
        <!-- image col -->
        <v-col cols="3" class="d-flex justify-center flex-column align-start  first-col">
          <img src="../assets/Vertical Capsule 748px x 896px.png" width="100%" class="rounded-xl" style=" border: 2px solid #265F67;" alt="">
          <p class="arabic-bold ma-2" style="font-size: 2rem;"> BLIND MEMORY </p>
          <p class="arabic-bold mx-2"> BY <a href="https://store.steampowered.com/curator/45736123" style="text-decoration: none;" target="_blank"> OliveRoots Studio </a> </p>
          <!-- <v-list dense flat rounded class="ml-n4">
            <v-list-item-group
              color="primary"
              class="arabic"
            >
              <v-list-item
              class="px-2"
                v-for="(item, i) in sideButtons"
                :key="i"
              >
                <v-list-item-content>
                  <v-list-item-title :to="item.to" class="mx-2 rounded-xl arabic rounded-xl">{{ item.text }}</v-list-item-title>
                </v-list-item-content>
              </v-list-item>
            </v-list-item-group>
          </v-list> -->
          <v-btn color="#29ABC5" class="rounded-xl arabic white--text ml-2" @click="downloadAll"><v-icon class="mx-2">mdi-download</v-icon> Download Images</v-btn>
        </v-col>
        <!-- Links -->
        <v-col cols="2" class="mr-5">
          <p class="arabic-bold ma-2" style="font-size: 2rem;"> Links </p>
          <p class="arabic-bold ma-2"> Platform: </p>
           <v-btn color="#1b2838" class="rounded-xl arabic white--text ma-2" href="https://store.steampowered.com/app/3894660/Blind_Memory/" target="_blank"> <v-icon class="mx-2">fa-brands fa-steam</v-icon> Steam </v-btn>
          <p class="arabic-bold ma-2"> Social Media: </p>
           <v-btn color="#ff0000"  rounded="xl" class="rounded-xl arabic white--text ma-2" href="https://www.youtube.com/@studiooliveroots/featured" target="_blank"><v-icon class="mx-2">fa-brands fa-youtube</v-icon> Youtube </v-btn> <br>
           <v-btn color="#13171A"  rounded="xl" class="rounded-xl arabic white--text ma-2" href="https://x.com/OliverootsStd?t=0rvTzcNTiaGBf-mwiIPPEw&s=09" target="_blank"><v-icon class="mx-2">fa-brands fa-x-twitter</v-icon> Twitter/X </v-btn> <br>
           <v-btn color="#7289DA"  rounded="xl" class="rounded-xl arabic white--text ma-2" href="https://discord.gg/5GGWHwhy" target="_blank"><v-icon class="mx-2">fa-brands fa-discord</v-icon> Discord </v-btn>
             <p class="arabic-bold ma-2"> Demo Release Date: </p>
             <p class="arabic ma-2">Steam | 13 October 2025 </p>
        </v-col>
        <v-col cols="6" class="ml-16">

              <p class="arabic-bold mb-3" style="font-size: 1.5rem;"> About This Game </p>
               <p class="arabic mb-5">
                  Blind Memory is an affluent experience to feel Lost, Chaos and Blinded.
                  You will play as Amnesiac and Half Blinded person who wakes up in a weird place knowing nothing about himself Nor about the place where a murder apparently took place.
                  So, Your choices now will shape your destiny—they’ll define who you are and how far you’ve come. But hold on tight… the journey’s just getting interesting, and the best surprises are yet to unfold.
               </p>

                 <p class="arabic-bold mb-3" style="font-size: 1.5rem;">Game Features </p>
                            <v-list-item>
                                <ul>
                                  <li class="arabic mb-1 ml-n2">Dual-Perspective Gameplay – Mix of 3D exploration + 2D scenes</li>
                                  <li class="arabic mb-1 ml-n2">Amnesia + Time Loops – unraveling mysteries</li>
                                  <li class="arabic mb-1 ml-n2">Atmospheric Horror – Focus on sound design & visual</li>
                                  <li class="arabic mb-1 ml-n2">Narrative Twists – mind-bending experience where nothing is as it seems.</li>
                                </ul>
                                </v-list-item>

        </v-col>
      </v-row>
      <v-divider class="ma-4"></v-divider>

      <v-row class="d-flex flex-column align-start justify-center">
        <v-col cols="12" class="d-flex flex-column align-start">
          <p class="arabic-bold ma-2" style="font-size: 2rem;"> Media</p>
          <p class="arabic ma-2">
            <span class="arabic-bold" style="font-size: 2rem;">Trailer |</span>
            Official Alpha Gameplay Trailer on
            <a href="https://www.youtube.com/watch?v=0Q4JvyuMB1w" target="_blank">Youtube</a>
          </p>
        </v-col>

      <v-col cols="12">
        <v-responsive class="rounded-xl" aspect-ratio="16/9" style="height: 600px;">
          <iframe
            width="100%"
            height="100%"
            src="https://www.youtube.com/embed/0Q4JvyuMB1w"
            title="Blind Memory - Official Alpha Gameplay Trailer | Mystery & Psychological Horror Title 2025"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
            allowfullscreen
          ></iframe>
        </v-responsive>
      </v-col>
      <v-col cols="12" class="d-flex flex-column align-start">
          <p class="arabic-bold ma-2" style="font-size: 2rem;"> Screenshots </p>
          <v-btn color="#29ABC5" class="rounded-xl arabic white--text ma-2" @click="downloadAll" ><v-icon class="mx-2" >mdi-download</v-icon> Download Images</v-btn>
<v-carousel
      hide-delimiter-background
      height="600"
      class="rounded-xl"
    >
      <v-carousel-item
        v-for="(screenshot, i) in screenshots"
        :key="i"
      >
        <v-img
          :src="screenshot"
          contain
          class="rounded-lg"
        ></v-img>
      </v-carousel-item>
    </v-carousel>
        </v-col>
      </v-row>
        <v-divider class="ma-4"></v-divider>
       <v-footer padless variant="absolute" color="transparent">
    <v-col
      class="text-center"
      cols="12"
    >
       <p class="arabic mx-16 text-center" style="font-size: small;" >
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
      link.href = '/Game Images/Game Images.zip' // path inside public
      link.download = 'Game Images.zip' // default filename
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
</style>
