<template>
  <footer class="py-5">
    <div class="container">
      <div class="row align-items-center h-vh-30 py-5">
        <div class="col-lg-12">
          <div class="wrapper">
            <div class="copyright d-block d-lg-flex justify-content-lg-between align-items-lg-center text-center">
              <ul class="text-uppercase d-inline mp-0">
                <li class="d-inline">
                  <router-link class="nav-link fs-7 fw-bold d-lg-inline d-block" to="#">content</router-link>
                </li>
                <li class="d-inline">
                  <router-link class="nav-link fs-7 fw-bold d-lg-inline d-block" to="#">conditions</router-link>
                </li>
              </ul>
              <div class="mb-5 mb-lg-0">
                <p class="mp-0">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quos, sed.</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComponent",
}
</script>