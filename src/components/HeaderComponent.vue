<template>
  <header class="min-vh-100 position-relative">
    <nav class="navbar fixed-top navbar-light px-4">
      <div class="container">
        <router-link class="navbar-brand text-center d-none d-lg-block text-uppercase mp-0 fw-bolder fs-5" to="#">
          34int
        </router-link>

        <button class="navbar-toggler mx-auto" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
          aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="navbar-brand d-flex justify-content-center align-items-center">
          <router-link class="text-decoration-none me-4 circle-icon" to="#"><i class="fas fa-share-alt"></i></router-link>
        </div>

        <div class="collapse navbar-collapse mt-3" id="navbarNav">
          <ul class="navbar-nav text-uppercase">
            <li class="nav-item px-0 px-lg-4">
              <router-link class="nav-link text-center" aria-current="page" to="#">work</router-link>
            </li>
            <li class="nav-item px-0 px-lg-4">
              <router-link class="nav-link text-center" to="#">home</router-link>
            </li>
            <li class="nav-item px-0 px-lg-4">
              <router-link class="nav-link text-center" to="#">about</router-link>
            </li>
            <li class="nav-item px-0 px-lg-4">
              <router-link class="nav-link text-center" to="#">contact</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <section>
      <div class="container">
        <div class="row min-vh-100 pt-5">
          <div class="col-lg-6">
            <div class="wrapper d-flex align-items-center h-100">
              <div class="w-100">
                <h1 class="text-navbar fw-normal mb-5">Projects</h1>
                <nav class="text-uppercase">
                  <router-link class="text-fade-1 text-decoration-none me-5" to="#">project</router-link>
                  <router-link class="text-fade-1 text-decoration-none me-5" to="#">services</router-link>
                  <router-link class="text-fade-1 text-decoration-none me-5" to="#">about</router-link>
                </nav>
              </div>
            </div>
          </div>
          <div class="col-lg-6">
            <div class="wrapper d-flex align-items-center h-100">
              <div class="w-100">
                <nav class="text-uppercase d-flex justify-content-between">
                  <div class="text">
                    <router-link class="text-fade-1 text-decoration-none d-block fw-bold mb-5" to="#">new york</router-link>
                    <router-link class="text-fade-1 text-decoration-none d-block fw-bold mb-5" to="#">london</router-link>
                  </div>
                  <div class="text">
                    <router-link class="text-fade-1 text-decoration-none d-block text-fade-black-1 mb-5" to="#">serang</router-link>
                    <router-link class="text-fade-1 text-decoration-none d-block fw-bold mb-5" to="#">spanyol</router-link>
                  </div>
                  <div class="text">
                    <router-link class="text-fade-1 text-decoration-none d-block fw-bold mb-5" to="#">argentina</router-link>
                    <router-link class="text-fade-1 text-decoration-none d-block text-fade-black-1 mb-5" to="#">indonesia</router-link>
                  </div>
                </nav>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
}
</script>

