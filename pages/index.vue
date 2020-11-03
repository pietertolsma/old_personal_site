<template>
  <div>
    <v-row class="particles">
      <v-col class="particle-col" cols="12" md="12">
        <vue-particles
        color="#dedede"
        :particleOpacity="0.7"
        :particlesNumber="180"
        shapeType="circle"
        :particleSize="4"
        linesColor="#dedede"
        :linesWidth="1"
        :lineLinked="true"
        :lineOpacity="0.4"
        :linesDistance="150"
        :moveSpeed="3"
        ></vue-particles>
      </v-col>
    </v-row>
    <v-container class="intro-cont">
      <v-row class="intro" justify="center" align="center">
        <v-col class="hello" lg="6" md="12" sm="12">
          <h1>Hi, I am Pieter.</h1>
        </v-col>
        <v-col class="profile-picture" lg="6" md="12" sm="12">
          <img src="~/assets/img/me.jpg" />
        </v-col>
      </v-row>
      <v-row>
        <v-col>
          <p>Lorem Ipsum. Lorem Ipsum. Lorem Ipsum. Lorem Ipsum. Lorem Ipsum. Lorem Ipsum. Lorem Ipsum. Lorem Ipsum. Lorem Ipsum. </p>
        </v-col>
      </v-row>
      <v-row class="projects-header-row">
        <v-col md="12" sm="12" cols="12" class="projects-header">
          <h1>Some of my Projects</h1>
        </v-col>
      </v-row>
      <v-row class="projects-row" no-gutter>
        <v-col class="project proj-nuna" lg="3" md="6" sm="6" xs="12">
          <a href="#" class="proj-in-cont">
            <div class="proj-background" />
            <div class="overlay">
              <h1>Nuna</h1>
            </div>
          </a>
        </v-col>
        <v-col class="project proj-air" lg="3" md="6" sm="6" xs="12">
          <a href="#" class="proj-in-cont">
            <div class="proj-background" />
            <div class="overlay">
              <h1>Operation AIR</h1>
            </div>
          </a>
        </v-col>
        <v-col class="project proj-psd2" lg="3" md="6" sm="6" xs="12">
          <a href="#" class="proj-in-cont">
            <div class="proj-background" />
            <div class="overlay">
              <h1>PSD2</h1>
            </div>
          </a>
        </v-col>
        <v-col class="project proj-tick" lg="3" md="6" sm="6" xs="12">
          <a href="#" class="proj-in-cont">
            <div class="proj-background" />
            <div class="overlay">
              <h1>Tickwave</h1>
            </div>
          </a>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style lang="scss">
.particles {
  padding: 0;
  margin: 0;
  height: 350px;
  position: absolute;
  top: 0;
  z-index: -1;
  background-color: #00b894;
  width: 100%;
  .particle-col {
    margin: 0;
    padding: 0;
  }
  #particles-js {
    margin: 0;
    padding: 0;
    height: 350px;
  }
}
.intro-cont {
  padding: 0;
}
.intro {
  z-index: 2;
  .hello {
    color: white;
    width: 100%;
    text-align: center;
    font-size: 2.3em;
    margin-top: 100px;
  }
  .profile-picture img{
    height: 350px;
    display: block;
    margin: 0 auto;
  }
}

.projects-header {
  text-align: center;
  margin: 30px 0;
  color: #00b894;
  font-size: 2em;
}

.projects-row {
  height: 200px;
  .project:hover .proj-background {
    transform: scale(1.2);
  }
  .project {
    .proj-in-cont {
      max-width: 400px;
      height: 200px;
      overflow: hidden;
      margin: 0 auto;
      display: block;
      text-decoration: none;
    }
    .proj-background {
      .z-index: 5;
      width: 100%;
      height: 100%;
      background-size: cover;
      transition: all .3s;
    }

    .overlay {
      z-index: 10;
      max-width: 400px;
      height: 200px;
      background-color: rgba(0, 184, 148, 0.5);
      position: relative;
      text-align: center;
      top: -200px;
      color: white;

      h1 {
        padding-top: 80px;
        width: 100%;
        height: 100%;
        text-align: center;
      }
    }
  }
  .proj-nuna {
    .proj-background {
      background-image: url('~assets/img/nunax.jpg');
    }
  }
  .proj-psd2 {
    .proj-background {
      background-image: url('~assets/img/psd2.jpg');
    }
  }
  .proj-tick {
    .proj-background {
      background-image: url('~assets/img/tickwave.jpg');
    }
  }
  .proj-air {
    .proj-background {
      background-image: url('~assets/img/operationair.jpg');
    }
  }
  .project {
    height: 200px;
    width: 300px;
    overflow: hidden;
    margin: 0;
    padding: 0;
  }
}
</style>
