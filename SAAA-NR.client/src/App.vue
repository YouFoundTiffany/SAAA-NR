<template>
  <header>
    <!-- moved Navbar out of Header into the main section -->
  </header>
  <main>
    <!-- STUB Banner Image SAAA is a Graphic, not text -->
    <section class="container-flex ban-con">
      <img src="src\assets\img\pollysgrouppic.jpg" alt="" class="bannerImg">
      <img src="src/assets/img/NorthernRockiesNameLogoWhiteDropShadRound.svg" alt=""
        class="animate__animated animate__backInDown center-that-img">
    </section>
    <!-- <h1 class="animate__animated animate__backInDown center-that-text text-light"
        style="text-align: center;position: absolute; top: 50%, left: 50% transform: translate:translate(-50%, -50%);">
        SAAA Northern
        Rockies</h1> -->

    <!-- STUB NAVBAR -->
    <Navbar />

    <!-- STUB Navbar -->
    <!-- <Navbar /> -->
    <!-- SPINNER -->
    <div v-if="loading" class="spin-contain">
      <div class="lds-spinner">
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
      </div>
    </div>
    <!-- SPINNER -->

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
    <!-- Modal -->


  </main>
  <footer class="m-0 p-2 bg-vista-blue text-light footerHorizontal">
    <!-- <div class="container"> -->
    <span class="justify-content-start text-start">©️SAAA Northern Rockies 2023</span>
    <!-- <span class="justify-content-end">Created By Renu Solutions</span> -->
    <!-- </div> -->
  </footer>
</template>

<script>
import { ref, onMounted } from 'vue'

export default {
  setup() {

    // SPINNER Define a reactive property for loading
    const loading = ref(true);

    onMounted(() => {

      // SPINNER Simulate a loading process
      setTimeout(() => {
        loading.value = false; // Set loading to false when the simulated loading process is done
      }, 1000);


    });

    return {
      loading
    };
  },
}
</script>


<style lang="scss">
.ban-con {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  /* Prevents any child elements from causing scroll */
}

.center-that-img {
  position: absolute;
  z-index: 10;
  /* Ensure the logo is above the other image */
  max-width: 100%;
  /* Limits the logo size to the container size */
  height: auto;
  /* Maintain aspect ratio */
}

.bannerImg {
  width: 100%;
  /* Assuming you want the banner image to span the width of the container */
  height: auto;
  /* Maintain aspect ratio */
}

/* Responsive adjustments for smaller screens */
@media screen and (max-width: 768px) {
  .center-that-img {
    max-width: 75%;
    /* Adjust the logo size on mobile */
  }
}



// .po-rel {
//   position: relative;
// }

// .center-that-img {
//   position: absolute center;


// }

// @media screen and (max-width: 768px) {
//   .center-that-img {
//     margin-left: auto;
//     margin-right: auto;
//     display: block;
//     left: 5%;
//   }
// }


.center-that-text {
  position: absolute;
  top: 50%;
  left: 35%;
  transform: translate(-50%, -50%);
  z-index: 2;
}

@media (max-width: 600px) {
  .center-that-text {
    left: 5%
  }
}

// Fly In Animation for Banner Text
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


// footer {
//   display: grid;
//   place-content: center;
//   height: 32px;
// }

// SCROLL UP BUTTON
#myBtn {
  display: none;
  /* Hidden by default */
  position: fixed;
  /* Fixed/sticky position */
  bottom: 20px;
  /* Place the button at the bottom of the page */
  right: 30px;
  /* Place the button 30px from the right */
  z-index: 99;
  /* Make sure it does not overlap */
  border: none;
  /* Remove borders */
  outline: none;
  /* Remove outline */
  background-color: red;
  /* Set a background color */
  color: white;
  /* Text color */
  cursor: pointer;
  /* Add a mouse pointer on hover */
  padding: 15px;
  /* Some padding */
  border-radius: 10px;
  /* Rounded corners */
  font-size: 18px;
  /* Increase font size */
}

#myBtn:hover {
  background-color: #555;
  /* Add a dark-grey background on hover */
}

// SCROLL UP BUTTON
</style>
