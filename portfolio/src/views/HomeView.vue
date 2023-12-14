<template>
  <v-app :style="{ background: $vuetify.theme.themes.dark.background}">
    <NavBar />
    <v-container fluid>
      <div class="secondchild1" id="home">
        <v-row>
          <v-col cols="6">
            <img class="pic" src="1.png">
          </v-col>
          <v-col cols="6" class="top">
            <h3>Hello, It's Me</h3>
            <h1>Swarnim Indraguru</h1>
            <vue-typed-js
             :strings="['Software Engineer', 'Developer', 'Coder', 'Problem Solver']"
             :typeSpeed="50"
             :startDelay="100"
             :backSpeed="100"
             :backDelay="100"
             :loop="true"
             :loopCount="50"
             :showCursor="false"
            >
              <h3>And I'm a <span class="typing"></span></h3>
            </vue-typed-js>
            <p class="grey--text">
              I'm a web developer with extensive experience for over 3 years.<br/>
              Experience in creat and develop website from both backend and frotend.<br/>
            </p>
            <v-btn tile color="red">Download CV</v-btn>
          </v-col>
        </v-row>
      </div>
      <div class="secondchild1" id="skills">
        <v-row>
          <v-col cols="6" class="skills">
            <h1>SKILLS</h1>
          </v-col>
          <v-col cols="6">
            <img src="java.svg">
            <img src="spring.svg">
            <img src="mysql.svg">
            <img src="vue.svg">
            <img src="html.svg">
            <img src="js.svg">
            <img src="css.svg">
            <img src="github.svg">
          </v-col>
        </v-row>
      </div>

      <div class="secondchild1" id="experience">
        <v-row>
          <v-col cols="6" class="skills">
            <h1>EXPERIENCE</h1>
            <v-col cols="6">
              <img src="capg.svg">
              <br>
              <br>
              <!-- <v-row row="2"> -->
                <img src="cg.png">
                <h5>Associate Consultant</h5>
              <!-- </v-row> -->
              <!-- <v-row row="2">
                <img src="cg.png">
                <h5>Associate Consultant</h5>
              </v-row>
              <v-row row="2">
                <img src="cg.png">
                <h5>Associate Consultant</h5>
              </v-row> -->
              <img src="cg.png">
              <h5>Senior Analyst</h5>
              <img src="cg.png">
              <h5>Analyst</h5>
            </v-col>
          </v-col>
        </v-row>
      </div>
      
      <div class="secondchild1" id="education">
        <v-row>
          <v-col cols="6" class="skills">
            <h1>EDUCATION</h1>
          </v-col>
        </v-row>
      </div>

      <div class="secondchild1" id="project">
        <v-row>
          <v-col cols="6" class="skills">
            <h1>PROJECTS</h1>
          </v-col>
        </v-row>
      </div>

      <v-row>
        <v-col>
          <v-col col="12" class="padd topInverse">
            <div class="second">
              <div class="secondchild1" id="contact">
                <v-row>
                  <v-col cols="7">
                    <h1 class="white--text">Lets work together on<br/>the next project</h1>
                    <p class="grey--text">
                      Will be happy to join you!!<br/>
                      tyrtuiojopugufughjlkiuythi98yguihdfuiho<br/>
                      tdyukliuyftgkhliouguytfglopiugiy
                    </p>
                  </v-col>
                  <v-col cols="5">
                    <v-btn tile color="#A7121D" dark class="mt-16" href="https://mail.google.com/mail/u/0/#inbox?compose=CllgCJNxNzVJzfpstcNxrRZglrqSMsPgTmhxfCBbxDwGVwPVzlXllzFKNqncSqfRjWQpQjHTDGq">Contact</v-btn>
                  </v-col>
                </v-row>
              </div>
            </div>
          </v-col>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
  import NavBar from '../components/NavBar'
  import Vue from 'vue'
  import VueTypedJs from 'vue-typed-js'

  Vue.use(VueTypedJs)

  export default {
    name: 'HomeView',

    components: {
      NavBar,
    },
  }
</script>

<style scoped>
.top{
  margin-top: 180px;
}
.typing{
  color:#ce1d2a;
}

.topInverse{
  margin-top: 550px;
}
.topTolbar{
  margin-top: 100px;
  text-align: center;
}
.first{
  width: 100%;
  height: 610px;
  background: linear-gradient(
    to right,
    #181818,
    #181818 50%,
    #111111 50%,
    #111111 50%,
  );
  text-align: center;
  padding: 2rem 2rem;
}
.second{
  width: 100%;
  height: 400px;
  background: #181818;
  text-align: center;
  padding: 2rem 2rem;
}
.secondchild {
  display: inline-block;
  background-color: #1e1e1e;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-top: 258px;
}

.skills{
  padding:250px 0px 0px 250px;

}
.child{
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
}
.bgColor1{
  background-color: #1e1e1e;
}

.bgColor2{
  background-color: #ce1d2a;
}
.child1{
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  width: 240px;
  margin-right: 5px;
}
.padding {
  padding: 12px 0 !important;
}
.col-12.padd{
  padding: 0 !important;;
}
.col-12.childcol{
  padding: 12px 0 !important;;
}
.h1.number{
  font-size: 50px;
  font-weight: bold;
}
</style>
