<template>
  <div id="app">

    <b-navbar toggleable="md" type="dark" variant="info" v-b-scrollspy fixed="top" class="bg-black">

      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>

      <b-navbar-brand href="#top"><img src="./assets/logo.png" /></b-navbar-brand>

      <b-collapse is-nav id="nav_collapse">

        <b-navbar-nav>
          <b-nav-item href="#logos"><a href="#logos" v-smooth-scroll>Logos</a></b-nav-item>
          <b-nav-item href="#colors"><a href="#colors" v-smooth-scroll>Colors</a></b-nav-item>
          <b-nav-item href="#fonts"><a href="#fonts" v-smooth-scroll>Fonts</a></b-nav-item>
          <b-nav-item href="#imagery"><a href="#imagery" v-smooth-scroll>Imagery</a></b-nav-item>
          <b-nav-item href="#messages"><a href="#messages" v-smooth-scroll>Messages</a></b-nav-item>
          <b-nav-item href="#marketing"><a href="#marketing" v-smooth-scroll>Marketing</a></b-nav-item>
          <b-nav-item href="#contact"><a href="#contact" v-smooth-scroll>Contact</a></b-nav-item>
        </b-navbar-nav>

      </b-collapse>
    </b-navbar>

    <router-view/>
    <back-to-top bottom="50px" right="50px">
      <button type="button" class="btn btn-info btn-to-top"><i class="fa fa-chevron-up"></i></button>
    </back-to-top>
    <div class="space"></div>
    <footer class="py-5 bg-black">
      <div class="container">
        <p class="m-0 text-center text-white small">Copyright &copy; Your Website 2018</p>
      </div>
      <!-- /.container -->
    </footer>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>

body {
  background: #f6f6f6;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.btn-to-top {
  width: 60px;
  height: 60px;
  padding: 10px 16px;
  border-radius: 50%;
  font-size: 22px;
  line-height: 22px;
  background: #000000;
}

a {
  color: #FFFFFF;
  text-transform: uppercase;
  font-weight: bold;
}

a:hover {
  text-decoration:none;
  color: #eeeeee;
}

.active a {
  color: #27a84a;
}

.space {
  width: 100%;
  height:600px;
}

/* theme styles */

.bg-black {
    background-color: #000!important
}

header.masthead {
    position: relative;
    overflow: hidden;
    padding-top: 20rem;
    padding-bottom: 20rem;
    background-image: url('./assets/SliderImage-ReGen1.jpg');
    background-repeat: no-repeat;
    background-position: center center;
    background-attachment: scroll;
    background-size: cover
}

header.masthead .masthead-content {
    z-index: 1;
    position: relative
}

header.masthead .masthead-content .masthead-heading {
    font-size: 4rem
}

header.masthead .masthead-content .masthead-subheading {
    font-size: 2rem
}

@media (min-width:992px) {
    header.masthead {
        padding-top: calc(10rem + 55px);
        padding-bottom: 10rem
    }
    header.masthead .masthead-content .masthead-heading {
        font-size: 6rem
    }
    header.masthead .masthead-content .masthead-subheading {
        font-size: 4rem
    }
}
</style>
