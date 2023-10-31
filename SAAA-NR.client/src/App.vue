<!-- APP.VUE -->
<template>
  <header>
    <!-- moved Navbar out of Header into the main section -->
  </header>
  <main>
    <!-- STUB Banner Image -->
    <section class="container-flex">
      <img src="src\assets\img\pollysgrouppic.jpg" alt="" class="bannerImg">
    </section>
    <Navbar />

    <!-- STUB Navbar -->
    <!-- <Navbar /> -->
    <router-view />
    <!-- Modal -->
    <div class="modal fade" id="TextOptIn" tabindex="-1" aria-labelledby="TextOptInLabel" aria-hidden="true">
      <div class="modal-dialog">
        <div class="modal-content">
          <div class="modal-header">
            <h1 class="modal-title fs-5" id="TextOptInLabel">Opt In for Texting</h1>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body">
            <!-- Modal -->
            <!-- STUB Texting Opt In Form -->
            <form id="#TextOptIn">
              <div class="mb-3">
                <label for="exampleInputEmail1" class="form-label">Email address</label>
                <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp">
                <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
              </div>
              <div class="mb-3">
                <label for="exampleInputPassword1" class="form-label">Password</label>
                <input type="password" class="form-control" id="exampleInputPassword1">
              </div>
              <div class="mb-3 form-check">
                <input type="checkbox" class="form-check-input" id="exampleCheck1">
                <label class="form-check-label" for="exampleCheck1">Check me out</label>
              </div>
              <button type="submit" class="btn text-light bg-vista-blue  textOptBtn">Submit</button>
            </form>





            <!-- Modal -->
          </div>
          <!-- <div class="modal-footer">
            <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
            <button type="button" class="btn btn-primary">Save changes</button>
          </div> -->
        </div>
      </div>
    </div>


  </main>
  <footer class="m-0 p-2 bg-vista-blue text-light footerHorizontal">
    <div class="container">
      <span class="justify-content-start text-start">©️SAAANR 2023</span>
      <!-- <span class="justify-content-end">Created By Renu Solutions</span> -->
    </div>
  </footer>
</template>

<script>
import { computed } from 'vue'
import { AppState } from './AppState'
// import Navbar from './components/Navbar.vue'

export default {
  setup() {
    return {
      appState: computed(() => AppState)
    }
  },
  // components: { Navbar }
}
</script>

<style lang="scss">
.textOptBtn:hover {
  background-color: var(--drkvista-blue) !important;
  color: white !important;
}

footer {
  padding: 1rem 0; // Add padding to the footer for aesthetic spacing
  height: auto; // Adjust height to fit content
}

// This ensures footer content is horizontally aligned on all screen sizes
.footerHorizontal {
  display: flex;
  justify-content: space-between; // This will space out the spans evenly
  flex-wrap: wrap; // Allows the spans to wrap on smaller screens if necessary
}

.footStart {
  justify-self: start;

}

.footEnd {
  justify-self: end;
}

.bannerImg {
  max-height: 50vh;
  width: 100%;
  object-fit: cover;
  object-position: center 25%;
  ;
}

@import "./assets/scss/main.scss";

:root {
  --main-height: calc(100vh - 32px - 64px);
}


footer {
  display: grid;
  place-content: center;
  height: 32px;
}
</style>
