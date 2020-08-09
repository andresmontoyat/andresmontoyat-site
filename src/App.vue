<template>
  <v-app app>
    <v-main>
      <v-container fluid>
        <v-row>
          <v-col cols="12">
            <v-row>
              <v-col cols="3">
                <v-card
                  class="mx-auto text-center rounded-lg"
                  height="600"
                  shaped>
                  <v-card-title>
                    <div id="inspire-profile-pic">
                      <v-tooltip bottom>
                        <template v-slot:activator="{ on }">
                          <v-avatar v-on="on" size="180">
                            <img
                              :src="require('./assets/me.jpg')"
                              alt="Me"
                            />
                          </v-avatar>
                        </template>
                        <span>H!, this is me</span>
                      </v-tooltip>
                    </div>
                  </v-card-title>
                  <v-card-text>
                    <div class="text-no-wrap">
                      <h3>Carlos A. Montoya Tob&oacute;n</h3>
                      <h4 class="subtitle-1">Solution Architect</h4>
                      <span>
                        <v-tooltip bottom>
                          <template v-slot:activator="{ on }">
                            <v-btn href="https://www.linkedin.com/in/carlos-andrés-montoya-tobón-8b508033/"
                              v-on="on" small tile fab icon color="blue">
                              <v-icon>fab fa-linkedin</v-icon>
                            </v-btn>
                          </template>
                          <span>LinkedIn</span>
                        </v-tooltip>
                        <v-tooltip bottom>
                          <template v-slot:activator="{ on }">
                            <v-btn href="https://github.com/andresmontoyat"
                              v-on="on" small tile fab icon color="black">
                              <v-icon>fab fa-github-alt</v-icon>
                            </v-btn>
                          </template>
                          <span>Github</span>
                        </v-tooltip>
                        <v-tooltip bottom>
                          <template v-slot:activator="{ on }">
                            <v-btn href="https://hub.docker.com/u/codehunters"
                              v-on="on" small tile fab icon color="blue">
                              <v-icon>fab fa-docker</v-icon>
                            </v-btn>
                          </template>
                          <span>Dockerhub</span>
                        </v-tooltip>
                        <v-tooltip bottom>
                          <template v-slot:activator="{ on }">
                            <v-btn href="https://www.youtube.com/channel/UCJ6I55Z9PMfuyoXNNVfn-RQ/featured?view_as=subscriber"
                              v-on="on" small tile fab icon color="red">
                              <v-icon>fab fa-youtube</v-icon>
                            </v-btn>
                          </template>
                          <span>Youtube</span>
                        </v-tooltip>
                      </span>
                    </div>
                  </v-card-text>
                </v-card>
              </v-col>
              <v-col cols="8">
                <v-card
                  class="mx-auto rounded-lg">
                  <v-carousel
                    v-model="inspCarouselContent"
                    height="600"
                    hide-delimiter-background
                    hide-delimiters>
                    <v-carousel-item :key="0">
                      <v-sheet
                        height="100%"
                        tile>
                        <v-row
                          class="fill-height"
                          align="center"
                          justify="center">
                          <div class="text-h4 text-center">
                            <p>Carlos Andres Montoya Tobon</p>
                            <p>Solution Architect</p>
                          </div>
                        </v-row>
                      </v-sheet>
                    </v-carousel-item>
                    <v-carousel-item :key="1">
                      <v-sheet
                        color="white"
                        height="100%"
                        tile>
                        <v-card
                          class="mx-auto"
                          height="100%">
                          <v-card-title class="text-h4">About me</v-card-title>
                          <v-card-text>
                            <v-row>
                              <v-col cols="6">
                                <p>Proin volutpat mauris ac pellentesque pharetra. Suspendisse congue elit vel odio suscipit, sit amet tempor nisl imperdiet. Quisque ex justo, faucibus ut mi in, condimentum finibus dolor. Aliquam vitae hendrerit dolor, eget imperdiet mauris. Maecenas et ante id ipsum condimentum dictum et vel massa. Ut in imperdiet dolor, vel consectetur dui.</p>
                              </v-col>
                              <v-col cols="6">
                                <ul>
                                  <li>
                                    <span class="title">Age</span>
                                    <span class="value">34</span>
                                  </li>
                                  <li>
                                    <span class="title">Residence</span>
                                    <span class="value">Colombia</span>
                                  </li>
                                  <li>
                                    <span class="title">Address</span>
                                    <span class="value">Santa Elena, Paysandu, Antioquia</span>
                                  </li>
                                  <li>
                                    <span class="title">E-mail</span>
                                    <span class="value">andresmontoyat@gmail.com</span>
                                  </li>
                                </ul>
                              </v-col>
                            </v-row>
                          </v-card-text>
                        </v-card>
                      </v-sheet>
                    </v-carousel-item>
                    <v-carousel-item :key="2">
                      <v-sheet
                        color="white"
                        height="100%"
                        tile>
                        <v-card
                          class="mx-auto"
                          height="100%">
                          <v-card-title class="text-h4">Resume</v-card-title>
                          <v-card-text>
                            <v-row>
                              <v-col cols="6">
                                <v-timeline>
                                <v-timeline-item
                                  v-for="n in 3"
                                  :key="n"
                                  color="red lighten-2"
                                  large
                                >
                                  <template v-slot:opposite>
                                    <span>Tus eu perfecto</span>
                                  </template>
                                  <v-card class="elevation-2">
                                    <v-card-title class="headline">Lorem ipsum</v-card-title>
                                    <v-card-text>
                                      Lorem ipsum dolor sit amet, no nam oblique veritus. Commune scaevola imperdiet nec ut, sed euismod convenire principes at. Est et nobis iisque percipit, an vim zril disputando voluptatibus, vix an salutandi sententiae.
                                    </v-card-text>
                                  </v-card>
                                </v-timeline-item>
                              </v-timeline>
                              </v-col>
                              <v-col cols="6">
                              </v-col>
                            </v-row>
                          </v-card-text>
                        </v-card>
                      </v-sheet>
                    </v-carousel-item>
                    <v-carousel-item :key="3">
                      <v-sheet
                        color="white"
                        height="100%"
                        tile>
                        <v-card
                          class="mx-auto"
                          height="100%">
                          <v-card-title class="text-h4">Contact</v-card-title>
                        </v-card>
                      </v-sheet>
                    </v-carousel-item>
                  </v-carousel>
                </v-card>
              </v-col>
              <v-col cols="1">
                <v-card
                  class="mx-auto rounded-lg"
                  tile>
                  <v-list>
                    <v-list-item>
                      <v-list-item-avatar>
                        <v-tooltip bottom>
                          <template v-slot:activator="{ on }">
                            <v-btn v-on="on" @click.stop="handleChangeCarousel(0)" class="ma-2" tile outlined fab color="blue">
                              <v-icon>fa fa-home</v-icon>
                            </v-btn>
                          </template>
                          <span>Home</span>
                        </v-tooltip>
                      </v-list-item-avatar>
                    </v-list-item>
                    <v-list-item>
                      <v-list-item-avatar>
                        <v-tooltip bottom>
                          <template v-slot:activator="{ on }">
                            <v-btn v-on="on" @click.stop="handleChangeCarousel(1)" class="ma-2" tile outlined fab color="blue">
                              <v-icon>fa fa-user-astronaut</v-icon>
                            </v-btn>
                          </template>
                          <span>About me</span>
                        </v-tooltip>
                      </v-list-item-avatar>
                    </v-list-item>
                    <v-list-item>
                     <v-list-item-avatar>
                       <v-tooltip bottom>
                          <template v-slot:activator="{ on }">
                            <v-btn v-on="on" @click.stop="handleChangeCarousel(2)" class="ma-2" tile outlined fab color="blue">
                              <v-icon>fa fa-rocket</v-icon>
                            </v-btn>
                          </template>
                          <span>Resume</span>
                       </v-tooltip>
                     </v-list-item-avatar>
                    </v-list-item>
                    <v-list-item>
                     <v-list-item-avatar>
                       <v-tooltip bottom>
                          <template v-slot:activator="{ on }">
                            <v-btn v-on="on" @click.stop="handleChangeCarousel(3)" class="ma-2" tile outlined fab color="blue">
                              <v-icon>fa fa-paper-plane</v-icon>
                            </v-btn>
                          </template>
                          <span>Contact</span>
                       </v-tooltip>
                     </v-list-item-avatar>
                    </v-list-item>
                  </v-list>
                </v-card>
              </v-col>
            </v-row>
          </v-col>
        </v-row>
      </v-container>
   </v-main>
  </v-app>
</template>
<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component({
  name: 'SiteVue'
})
export default class SiteVue extends Vue {
  inspCarouselContent = 0

  handleChangeCarousel (index: number): void {
    this.inspCarouselContent = index
  }
}
</script>
<style scoped>
#inspire-profile-pic {
  display: block;
  margin-left: auto;
  margin-right: auto
}
</style>
