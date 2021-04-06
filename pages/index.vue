<template>
  <div class="">
    <div
      class="paralax ma-0 pa-0"
      :style="{ backgroundImage: `url(${image})` }"
      style="position: relative"
    >
      <template>
        <v-carousel hide-delimiter-background delimiter-position="top" cycle interval="2000">
          <v-carousel-item>
            <v-sheet height="100%" tile>
              <v-row class="fill-height text-left px-lg-16 px-5 pt-16 mx-0">
                <v-col
                  class="text-center my-auto px-md-16 px-sm-10 px-xs-5 pt-md-16 pt-sm-10"
                  cols="12"
                  lg="6"
                  md="10"
                >
                  <h1 class="font-weight-bold mb-4 text-left white--text">
                    Your Story Starts With Us.
                  </h1>
                  <h4 class="subheading font-weight-thin text-left white--text">
                    Every landing page needs a small description after the big
                    bold title, that's why we added this text here. Add here all
                    the information that can make you or your product create the
                    first impression.
                  </h4>
                  <nuxt-link
                    to="/sample"
                    color="error"
                    class="text-decoration-none btn-error float-left mt-md-10 mt-5"
                  >
                    <v-icon class="mr-1" color="white">mdi-play</v-icon>
                    WATCH VIDEO
                  </nuxt-link>
                </v-col>
              </v-row>
            </v-sheet>
          </v-carousel-item>
          <v-carousel-item>
            <v-sheet height="100%" tile>
              <v-row class="fill-height text-left px-lg-16 px-5 pt-16 mx-0">
                <v-col
                  class="text-center my-auto px-md-16 px-sm-10 px-xs-5 pt-md-16 pt-sm-10"
                  cols="12"
                  lg="6"
                  md="10"
                >
                  <h1 class="font-weight-bold mb-4 text-left white--text">
                    Your Story Starts With Us.
                  </h1>
                  <h4 class="subheading font-weight-thin text-left white--text">
                    Every landing page needs a small description after the big
                    bold title, that's why we added this text here. Add here all
                    the information that can make you or your product create the
                    first impression.
                  </h4>
                  <nuxt-link
                    to="/sample"
                    color="error"
                    class="text-decoration-none btn-error float-left mt-md-10 mt-5"
                  >
                    <v-icon class="mr-1" color="white">mdi-play</v-icon>
                    WATCH VIDEO
                  </nuxt-link>
                </v-col>
              </v-row>
            </v-sheet>
          </v-carousel-item>
          <v-carousel-item>
            <v-sheet height="100%" tile>
              <v-row class="fill-height text-left px-lg-16 px-5 pt-16 mx-0">
                <v-col
                  class="text-center my-auto px-md-16 px-sm-10 px-xs-5 pt-md-16 pt-sm-10"
                  cols="12"
                  lg="6"
                  md="10"
                >
                  <h1 class="font-weight-bold mb-4 text-left white--text">
                    Your Story Starts With Us.
                  </h1>
                  <h4 class="subheading font-weight-thin text-left white--text">
                    Every landing page needs a small description after the big
                    bold title, that's why we added this text here. Add here all
                    the information that can make you or your product create the
                    first impression.
                  </h4>
                  <nuxt-link
                    to="/sample"
                    color="error"
                    class="text-decoration-none btn-error float-left mt-md-10 mt-5"
                  >
                    <v-icon class="mr-1" color="white">mdi-play</v-icon>
                    WATCH VIDEO
                  </nuxt-link>
                </v-col>
              </v-row>
            </v-sheet>
          </v-carousel-item>
        </v-carousel>
      </template>
    </div>

    <div class="mt-n16 px-md-8 px-4">
      <v-card class="rounded-lg px-sm-8 px-4 py-10" color="white" elevation="8">
        <v-row no-gutters justify="center">
          <v-col cols="12" md="8" class="text-center pt-10">
            <h2>Let's talk product</h2>
            <h5 class="text-grey">
              This is the paragraph where you can write more details about your
              product. Keep you user engaged by providing meaningful
              information. Remember that by this time, the user is curious,
              otherwise he wouldn't scroll to get here. Add a button if you want
              the user to see more.
            </h5>
          </v-col>
        </v-row>
        <v-row no-gutters class="px-sm-8 px-0 pt-5 pb-10">
          <v-col cols="12" md="4">
            <v-card class="pa-2 border-0 text-center pa-7" outlined tile>
              <v-icon class="" style="font-size: 61px; color: #00acc1"
                >mdi-message-text</v-icon
              >
              <h4 class="my-4">Free Chat</h4>
              <p>
                Divide details about your product or agency work into parts.
                Write a few lines about each one. A paragraph describing a
                feature will be enough.
              </p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card class="pa-2 border-0 text-center pa-7" outlined tile>
              <v-icon class="" style="font-size: 61px; color: #4caf50"
                >mdi-shield-check</v-icon
              >
              <h4 class="my-4">Verified Users</h4>
              <p>
                Divide details about your product or agency work into parts.
                Write a few lines about each one. A paragraph describing a
                feature will be enough.
              </p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4">
            <v-card class="pa-2 border-0 text-center pa-7" outlined tile>
              <v-icon class="" style="font-size: 61px; color: #f44336"
                >mdi-fingerprint</v-icon
              >
              <h4 class="my-4">Fingerprint</h4>
              <p>
                Divide details about your product or agency work into parts.
                Write a few lines about each one. A paragraph describing a
                feature will be enough.
              </p>
            </v-card>
          </v-col>
        </v-row>
      </v-card>
    </div>
    <div class="mt-16 px-md-8 px-4">
      <v-card
        class="rounded-lg px-sm-8 px-4 py-10"
        color="grey lighten-4"
        elevation="8"
      >
        <v-row no-gutters class="px-sm-8 px-0 py-sm-16 py-0">
          <v-col cols="12" md="12" class="text-center">
            <v-row justify="center">
              <v-col cols="12" md="7">
                <h2 style="color: rgb(0, 188, 212)">How can we help?</h2>
                <h3 class="text-grey">
                  TheCompany Data is a professional services firm with over 20
                  years of Software Development and BI experience. <br />
                  We put that experience to work for you and get actionable
                  insights in <i>days or weeks</i> - not months.
                </h3>
              </v-col>
            </v-row>
          </v-col>
          <v-col cols="12" md="4" class="pa-1 pa-md-5 mt-5">
            <v-card
              class="border-0 text-center px-sm-3 px-1 py-10 rounded-lg"
              color="white"
              outlined
              tile
              elevation="3"

            >
              <v-icon class="my-3" style="font-size: 61px; color: #00acc1"
                >mdi-cloud-download-outline</v-icon
              >
              <h4 class="my-4">Data Extraction & Integration</h4>
              <p>
                First, we partner with client stakeholders to identify key data
                sources and get to work extracting and coalescing your data from
                vendor API's, nosql and traditional sql databases and yes, all
                your excel files too ;)
              </p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4" class="pa-1 pa-md-5 mt-5">
            <v-card
              class="border-0 text-center px-sm-3 px-1  py-10 rounded-lg"
              color="white"
              outlined
              elevation="3"
              tile
            >
              <v-icon class="my-3" style="font-size: 61px; color: #4caf50 "
                >mdi-view-dashboard-outline</v-icon
              >
              <h4 class="my-4">Reporting & Data Visualization</h4>
              <p>
                Next, we craft reports to help you where it's hurting. It's
                critical to start building the reports as early as possible to
                prime the creative process and produce enough iterations for the
                cream to rise to the top. The early results of this step usually
                produce quite a bit of excitement and tend to add momentum to
                the project.
              </p>
            </v-card>
          </v-col>
          <v-col cols="12" md="4" class="pa-1 pa-md-5 mt-5">
            <v-card
              class="border-0 text-center px-sm-3 px-1  py-10 rounded-lg"
              color="white"
              outlined
              elevation="3"
              tile
            >
              <v-icon class="my-2" style="font-size: 61px; color: #00acc1"
                >mdi-gesture-tap</v-icon
              >
              <h4 class="my-4">Automation</h4>
              <p>
                We then automate the data collection process and refine reports
                into reporting dashboards and storyboards that your C team and
                management can use to drive their strategic decision making
                processes across the organization.
              </p>
            </v-card>
          </v-col>
        </v-row>
        <v-row no-gutters class="px-sm-8 px-0 py-md-16 py-0" justify="center">
          <v-col cols="12" md="8" class="text-center">
            <h2>Work with us</h2>
            <h4 class="text-grey font-weight-light pa-5">
              Divide details about your product or agency work into parts. Write
              a few lines about each one and contact us about any further
              collaboration. We will responde get back to you in a couple of
              hours.
            </h4>
          </v-col>
          <v-col cols="12" md="8" class="px-6">
            <v-form ref="form" v-model="valid" lazy-validation>
              <v-row>
                <v-col cols="12" md="6">
                  <v-text-field
                    v-model="name"
                    :rules="nameRules"
                    label="Name"
                    required
                  ></v-text-field>
                </v-col>
                <v-col cols="12" md="6">
                  <v-text-field
                    v-model="email"
                    :rules="emailRules"
                    label="E-mail"
                    required
                  ></v-text-field>
                </v-col>
                <v-col cols="12">
                  <v-textarea
                    autocomplete="Your Message"
                    label="Your Message"
                  ></v-textarea>
                </v-col>
                <v-col cols="12">
                  <v-btn class="white--text bg-light pa-5" color="purple">
                    SEND MESSAGE
                  </v-btn>
                </v-col>
              </v-row>
            </v-form>
          </v-col>
        </v-row>
      </v-card>
    </div>
  </div>
</template>


<script>
import bgimage from 'assets/images/landing-bg.jpg'

export default {
  data() {
    return {
      image: bgimage,
      layout: 'default',
      extraNavClasses: '',
      toggledClass: false,
      valid: true,
      name: '',
      nameRules: [
        (v) => !!v || 'Name is required',
        (v) => (v && v.length <= 10) || 'Name must be less than 10 characters',
      ],
      email: '',
      emailRules: [
        (v) => !!v || 'E-mail is required',
        (v) => /.+@.+\..+/.test(v) || 'E-mail must be valid',
      ],
    }
  },
  methods: {
    validate() {
      this.$refs.form.validate()
    },
    reset() {
      this.$refs.form.reset()
    },
    resetValidation() {
      this.$refs.form.resetValidation()
    },
  },
}
</script>
<style scoped lang="scss">
.paralax {
  min-height: 90vh;

  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.theme--dark.v-sheet {
  background-color: transparent !important;
}

h1 {
  font-size: 3.3125rem !important;
  line-height: 1.15em !important;
  font-family: 'Roboto Slab ' !important;
}
h3 {
  font-size: 1.5625rem;
  line-height: 1.4em;
  font-weight: 300;
}
h4 {
  font-size: 1.125rem !important;
  line-height: 1.5em !important;
  color:#3C4858
}
.v-parallax {
  position: relative;
  overflow: hidden;
  z-index: 0;
  height: 90vh !important;
}
.btn-error {
  padding: 1.125rem 2.25rem;
  font-size: 0.875rem;
  line-height: 1.333333;
  border-radius: 0.2rem;
  background-color: #f44336;
  color: white;
}
h2 {
  color: #3c4858;
  margin: 1.75rem 0 0.875rem;
  margin-top: 30px;
  min-height: 32px;
  font-family: 'Roboto Slab', 'Times New Roman', serif;
  font-weight: 700;
  margin-bottom: 1rem;
  font-size: 2.25rem;
  line-height: 1.5em;
}
.text-grey {
  color: #999;
}
h5 {
  font-size: 1.0625rem;
  line-height: 1.55em;
  font-weight: 300;
}
.border-0 {
  border: none;
}
p {
  color: #999999;
  overflow: hidden;
  font-size: 14px;
  margin-top: 0px;
  margin: 0 0 10px;
}
small {
  font-weight: 400;
  font-size: 75%;
  color: #6c757d;
}
.h-100 {
  height: 100%;
}
.w-50 {
  width: 50%;
}
.v-parallax__image-container {
  position: inherit !important;
}
.v-parallax__image {
  display: none !important;
}
@media (max-width: 490px) {
  h1 {
    font-size: 2rem !important;
  }
  .btn-error[data-v-2a183b29] {
    padding: 0.5rem 0.5rem;
  }
   h3 {
    font-size: 1.20rem !important;
  }
}
@media (max-width: 375px) {
  h2 {
    font-size: 2rem !important;
  }
  h3 {
    font-size: 1rem !important;
  }
  .btn-error[data-v-2a183b29] {
    padding: 0.5rem 0.5rem;
  }
}
</style>