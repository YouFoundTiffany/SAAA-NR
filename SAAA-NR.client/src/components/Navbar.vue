<!-- NAVBAR -->
<template>
  <!-- TODO figure out sticky fixed-top navbar that still sits under the banner image.  -->
  <nav class="navbar navbar-expand-lg px-3 border-bottom border-5 border-drkvista-blue blue-gradient-top">
    <!-- <router-link class="navbar-brand navbar-show navbar-show d-flex mobileHome" :to="{ name: 'Home' }">
      <div class="d-flex flex-column align-items-center">
        <img alt="logo" src="src\assets\img\SAAALogoSmall.svg" height="45" />
      </div>
    </router-link> -->
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarText"
      aria-controls="navbarText" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse text-center justify-content-center px-2" id="navbarText"
      style="list-style-type: none">
      <router-link class="navbar-brand d-flex fullscrnHome" :to="{ name: 'Home' }">
        <div class="d-flex flex-column align-items-center">
          <img alt="logo" src="src\assets\img\SAAALogoSmall.svg" height="45" title="Home Page" />
        </div>
      </router-link>
      <li>
        <router-link :to="{ name: 'Events' }"
          class="btn lighten-30 selectable text-uppercase fw-bold text-ultra-drkvista-blue">
          Events
        </router-link>
      </li>
      <li>
        <router-link :to="{ name: 'Practices' }"
          class="btn lighten-30 selectable text-uppercase fw-bold text-ultra-drkvista-blue">
          Practices
        </router-link>
      </li>
      <li>
        <router-link :to="{ name: 'About' }"
          class="btn lighten-30 selectable text-uppercase fw-bold text-ultra-drkvista-blue">
          About SAAA-NR
        </router-link>
      </li>
      <li>
        <router-link :to="{ name: 'Games History' }"
          class="btn lighten-30 selectable text-uppercase fw-bold text-ultra-drkvista-blue">
          Games History
        </router-link>
      </li>
      <li>
        <a class="btn lighten-30 selectable text-uppercase fw-bold text-ultra-drkvista-blue px-2"
          href="https://scottishscores.com/" target="_blank">Scottish
          Scores</a>
      </li>

      <!-- STUB dropdown -->
      <div class="dropdown">
        <button class="btn lighten-30 selectable dropdown-toggle text-uppercase fw-bold text-ultra-drkvista-blue"
          type="button" data-bs-toggle="dropdown" aria-expanded="false">
          More Info
        </button>
        <ul class="dropdown-menu">
          <li><a class="dropdown-item text-uppercase fw-bold text-ultra-drkvista-blue"
              href="https://www.saaa-national.org/" target="_blank">SAAA-National</a></li>
          <li><a class="dropdown-item text-uppercase fw-bold text-ultra-drkvista-blue"
              href="https://www.saaa-national.org/_files/ugd/a42bbf_5ccc511a23024e32bf7252d7945fd65d.pdf"
              target="_blank">SAAA-National
              Rules</a>
          </li>
          <li><a class="dropdown-item text-uppercase fw-bold text-ultra-drkvista-blue"
              href="https://www.saaa-national.org/information" target="_blank">NASGA</a></li>
          <li>
            <a type="button" class="btn bg-vista-blue text-light textOptBtn" data-bs-toggle="modal"
              data-bs-target="#TextOptIn">Sign
              Up for Text Notificaitons</a>
          </li>
        </ul>
      </div>

    </div>
    <!-- LOGIN COMPONENT HERE -->
    <!-- <Login /> -->
  </nav>
</template>

<script>
// import Login from './Login.vue';
export default {
  setup() {
    return {}
  },
  // components: { Login }
}
</script>

<style scoped>
@media (min-width: 600px) {
  .navbar-brand {
    display: none;
    /* Hide the top div on larger screens */
  }

  nav {
    height: 64px;
  }
}

/* Styles that will apply to all sizes */
.navbar-nav .router-link-exact-active {
  border-bottom: 2px solid;
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0;
  list-style-type: none;
}

.textOptBtn:hover {
  background-color: var(--drkvista-blue);
  color: white;
}

/* Hide the mobile home link on larger screens */
@media(min-width: 600px) {
  .mobileHome {
    display: none;
  }

  /* Ensuring the full screen home link displays on larger screens */
  .fullscrnHome {
    display: flex;
  }

  nav {
    height: 64px;
  }
}

/* Hide the full screen home link on smaller screens */
@media (max-width: 600px) {
  .fullscrnHome {
    display: none;
  }

  /* Ensuring the mobile home link displays on smaller screens */
  .mobileHome {
    display: flex;
  }
}
</style>

