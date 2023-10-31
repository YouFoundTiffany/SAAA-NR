<template>
  <div class="container text-center">
    <h1>Practices</h1>
    <p>more detils</p>
    <p>more detils</p>
  </div>
  <!-- STUB Texting Opt In Modal -->
  <!-- Button trigger modal -->
  <section class="container d-flex justify-content-center align-items-center">
    <button type="button" class="btn bg-vista-blue text-light text-center textOptBtn" data-bs-toggle="modal"
      data-bs-target="#TextOptIn">
      Sign Up for Text Notifications</button>
  </section>
  <!-- STUB Border -->
  <div class="container py-3">
    <div class="border border-top border-vista-blue"></div>
  </div>


  <!-- STUB half and half Card -->
  <!-- <section class="container-flex pt-3"> -->

  <!-- Left -->
  <!-- <h5 class="card-title text-end pe-5">LETS PUT THE UPCOMING EVENT HERE</h5>
    <div class="container" style="margin-top: -10vh; margin-bottom: -12vh;">
      <div class="row">
        <div class="col-12 col-md-6">
          <div class=" text-center">
            <img src="src\assets\img\SAAALogoMed.svg" class="card-img-top" alt="Logo">
          </div>
        </div> -->

  <!-- Right -->
  <!-- <div class="col-12 col-md-6 d-flex align-items-center">
          <div class=" text-center w-100">
            <div class="card-body">
              <p class="card-text">Your Property in Good Hands.</p>
              <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipiscing elit...</p>
            </div>
          </div>
        </div>
      </div>
    </div> -->
  <!-- </section> -->
</template>

<script>
export default {
  setup() {
    return {

    }
  }
}
</script>
<style scoped lang="scss">
.textOptBtn:hover {
  background-color: var(--drkvista-blue);
  color: white;
}
</style>
