<!-- HOME PAGE -->
<template>
  <!-- STUB half and half Card -->
  <section class="container-flex py-5">
    <!-- Left -->
    <h5 class="card-title text-center pe-md-5 next-event">NEXT EVENT</h5>
    <div class="container" style="margin-top: -10vh; margin-bottom: -12vh;">
      <div class="row">
        <div class="col-12 col-md-6">
          <div class=" text-center">
            <img src="src\assets\img\SAAALogoMed.svg" class="card-img-top" alt="Logo">
          </div>
        </div>

        <!-- Right -->
        <div class="col-12 col-md-6 d-flex align-items-center">
          <div class=" text-center w-100">
            <div class="card-body">
              <h5 class="card-title text-center pe-5">Frozen Stones</h5>
              <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni, doloribus!.</p>
              <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- STUB Border -->
  <div class="container py-4">
    <div class="border border-top border-vista-blue"></div>
  </div>

  <!-- STUB 3 Cards w header and description section-->
  <section class="container-flex m-2">

    <!-- Card 1 -->
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-md-6 mb-4">
          <div class="card text-center h-90vh">
            <img src="src\assets\img\Titan21.jpg" class="card-img-top img-fluid" alt="...">
            <div class="card-body">
              <h5 class="card-title">SKILLED PROFESSIONALS.</h5>
              <p class="card-text">Your Property in Good Hands.</p>
              <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
            </div>
          </div>
        </div>

        <!-- Card 2 -->
        <div class="col-lg-4 col-md-6 mb-4">
          <div class="card text-center h-90vh">
            <img src="src\assets\img\SAAALogoMed.svg" class="card-img-top img-fluid" alt="...">
            <div class="card-body">
              <h5 class="card-title">SKILLED PROFESSIONALS.</h5>
              <p class="card-text">Your Property in Good Hands.</p>
              <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
            </div>
          </div>
        </div>

        <!-- Card 3 -->
        <div class="col-lg-4 col-md-6 mb-4 ">
          <div class="card text-center h-90vh">
            <img src="src\assets\img\chrismoore.jpg" class="card-img-top img-fluid" alt="...">
            <div class="card-body">
              <h5 class="card-title">SKILLED PROFESSIONALS.</h5>
              <p class="card-text">Your Property in Good Hands.</p>
              <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
            </div>
          </div>
        </div>
        <!-- Repeat the above col-md-4 div for each card you want to display -->
      </div>
    </div>
  </section>


  <!-- STUB Color and text in Section -->
  <section class="container-flex m-2 logobnw">
    <img class="bnw rsizeImgHP1" src="src/assets/img/SAAALogoMed.svg" alt="Logo">
    <div class="overlay"></div>
    <h1 class="text">Your Text Here</h1>
  </section>




  <!-- STUB Pre-Footer -->
  <section class="container-flex m-2">




  </section>
</template>

<script>
export default {

  setup() {
    return {}
  }
}
</script>

<style scoped lang="scss">
// section
.h-90vh {
  height: 90vh;
  /* Set the height of the cards */
}

.card-img-top {
  height: 50%;
  /* Adjust based on your preference */
  object-fit: cover;
  /* Ensure images cover the area without distortion */
}

.logobnw {
  position: relative;
  /* Set your desired width and height */
}


// section
.rsizeImgHP1 {
  height: 25vh !important;
  width: 100%;
  object-fit: auto;
  object-position: center 25%
}


// section

.bnw {
  filter: grayscale(100%);
  width: 100%;
  height: 100%;
  /* Ensure the SVG fills the container */
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: rgba(129, 168, 230, 0.432);
  /* Black with 50% opacity */
  z-index: 1;
  /* Overlay should be above the SVG */
}

.text {
  position: absolute;
  top: 50%;
  /* Center the text vertically */
  left: 50%;
  /* Center the text horizontally */
  transform: translate(-50%, -50%);
  /* Offset the text by its own size to center */
  z-index: 2;
  /* Text should be on top of the overlay */
  color: white;
  /* Choose text color that is visible over the overlay */
  /* Add more styling as needed */
}

// section
.bannerImg {
  max-height: 50vh;
  width: 100%;
  object-fit: cover;
  object-position: center 25%;
  ;
}

// FIXME
@media (min-width: 600px) {
  .next-event {
    margin: 20px;
    /* Hide the top div on larger screens */
  }


}
</style>
