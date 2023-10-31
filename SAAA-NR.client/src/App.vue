<!-- APP.VUE -->
<template>
  <header>
    <!-- moved Navbar out of Header into the main section -->
  </header>
  <main>
    <!-- STUB Banner Image -->
    <section class="container-flex position-relative fyIn-container">
      <h1 class="animate__animated animate__backInDown center-that-text text-light"
        style="text-align: center;position: absolute; top: 50%, left: 50% transform: translate:translate(-50%, -50%);">
        SAAA Northern
        Rockies</h1>
      <img src="src\assets\img\pollysgrouppic.jpg" alt="" class="bannerImg">
    </section>
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


  </main>
  <footer class="m-0 p-2 bg-vista-blue text-light footerHorizontal">
    <div class="container">
      <span class="justify-content-start text-start">©️SAAA Northern Rockies 2023</span>
      <!-- <span class="justify-content-end">Created By Renu Solutions</span> -->
    </div>
  </footer>
  <!-- </section>============================== -->
  <!-- Footer Area -->
  <!-- ============================== -->
  <!-- <footer class="footer-wrapper footer-layout1">
        <div class="footer-top">
            <div class="container">
                <div class="row align-items-stretch">
                    <div class="col-md-4 d-none d-lg-flex">
                        <div class="social-style2">
                            <a href="#"><i class="fab fa-facebook-f"></i></a>
                            <a href="#"><i class="fab fa-twitter"></i></a>
                            <a href="#"><i class="fab fa-instagram"></i></a>
                            <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        </div>
                    </div>
                    <div class="col-md-5 col-lg-4">
                        <div class="vs-logo">
                            <a href="index.html"><img src="assets/img/logo-2.svg" alt="logo"></a>
                        </div>
                    </div>
                    <div class="col-md-7 col-lg-4">
                        <form action="#" class="form-style1">
                            <h3 class="form-title">Our newsletter</h3>
                            <div class="form-group">
                                <input type="email" placeholder="Enter your email...">
                                <button class="vs-btn" type="submit">Subscribe</button>
                            </div>
                        </form>
                    </div>
                </div>
            </div>
        </div>
        <div class="widget-area">
            <div class="container">
                <div class="row justify-content-between">
                    <div class="col-md-6 col-xl-auto">
                        <div class="widget footer-widget">
                            <h3 class="widget_title">About Wellnez</h3>
                            <p class="footer-info"><i class="fal fa-map-marker-alt text-theme me-2"></i> Centerl Park West La, New York <br> <a href="tel:+01234567890" class="text-inherit"><i class="far fa-phone-alt text-theme me-2"></i>+0 123 456 7890</a> <br> <a class="text-inherit" href="mailto:info@example.com"><i class="fal fa-envelope text-theme me-2"></i>info@example.com</a> </p>
                            <h4 class="fs-22 mb-2">Open Hours</h4>
                            <p class="footer-time">Sunday to Friday <span class="time">08:00 - 20:00</span></p>
                        </div>
                    </div>
                    <div class="col-md-6 col-xl-auto">
                        <div class="widget widget_nav_menu  footer-widget">
                            <h3 class="widget_title">Important Links</h3>
                            <div class="menu-all-pages-container footer-menu">
                                <ul class="menu">
                                    <li><a href="service.html">Serivces</a></li>
                                    <li><a href="about.html">ABOUT US</a></li>
                                    <li><a href="price-plan.html">Price Plan</a></li>
                                    <li><a href="contact.html">CONTACT</a></li>
                                    <li><a href="blog.html">Our Blog</a></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6 col-xl-auto">
                        <div class="widget widget_nav_menu  footer-widget">
                            <h3 class="widget_title">CATEGORIES</h3>
                            <div class="menu-all-pages-container footer-menu">
                                <ul class="menu">
                                    <li><a href="service.html">SKINCARE</a></li>
                                    <li><a href="service.html">MAKEUP</a></li>
                                    <li><a href="service.html">FRAGRANCE</a></li>
                                    <li><a href="service.html">HAIRCARE</a></li>
                                    <li><a href="service.html">BATH & BODY</a></li>
                                </ul>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-6 col-xl-auto">
                        <div class="widget footer-widget">
                            <h3 class="widget_title">Recent Post</h3>
                            <div class="recent-post-wrap">
                                <div class="recent-post">
                                    <div class="media-img">
                                        <a href="blog-details.html"><img src="assets/img/widget/recent-post-2-1.jpg" alt="Blog Image"></a>
                                    </div>
                                    <div class="media-body">
                                        <h4 class="post-title"><a class="text-inherit" href="blog-details.html">Managing Partner along</a></h4>
                                        <div class="recent-post-meta">
                                            <a href="blog.html"><i class="fas fa-calendar-alt"></i>05 AUG, 2023</a>
                                        </div>
                                    </div>
                                </div>
                                <div class="recent-post">
                                    <div class="media-img">
                                        <a href="blog-details.html"><img src="assets/img/widget/recent-post-2-2.jpg" alt="Blog Image"></a>
                                    </div>
                                    <div class="media-body">
                                        <h4 class="post-title"><a class="text-inherit" href="blog-details.html">Senior Counsels. Partnr along</a></h4>
                                        <div class="recent-post-meta">
                                            <a href="blog.html"><i class="fas fa-calendar-alt"></i>11 AUG, 2023</a>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="copyright-wrap">
            <div class="container">
                <div class="row justify-content-between align-items-center">
                    <div class="col-md-auto text-center">
                        <p class="copyright-text">Copyright <i class="fal fa-copyright"></i> 2023 <a href="index.html">Wellnez</a>. All Rights Reserved By <a href="https://themeforest.net/user/vecuro_themes">Vecuro</a></p>
                    </div>
                    <div class="col-auto d-none d-md-block">
                        <img src="assets/img/widget/cards.png" alt="cards">
                    </div>
                </div>
            </div>
        </div>
    </footer>  Scroll To Top -->
  <!-- from template <a href="#" class="scrollToTop scroll-btn"><i class="far fa-arrow-up"></i></a> -->



  <!-- SCROLL UP BUTTON that I copied from somewhere-->
  <!-- <button onclick="topFunction()" id="myBtn" title="Go to top">Top</button> -->
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
// Fly In Animation for Banner Text
.fyIn-container {
  position: relative;
}

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
