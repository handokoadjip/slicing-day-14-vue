<template>
  <HeaderComponent />
  <main>
    <router-view />
  </main>
  <FooterComponent />
</template>

<script>
import $ from 'jquery';
import HeaderComponent from "@/components/HeaderComponent.vue"
import FooterComponent from "@/components/FooterComponent.vue"

export default {
  name: 'App',
  components: {
    HeaderComponent,
    FooterComponent
  },
  mounted: function() {
    $(document).ready(function() {
      function mobileViewUpdate() {
        const viewportWidth = $(window).width();
        if(viewportWidth < 600) {
          $(".navbar.fixed-top").addClass("scrolled");
          $(".navbar-brand").addClass("scrolled");
        } else {
          $(document).scroll(function() {
            const nav = $(".navbar.fixed-top");
            const brand = $(".navbar-brand");
            nav.toggleClass("scrolled", $(this).scrollTop() > nav.height());
            brand.toggleClass("scrolled", $(this).scrollTop() > nav.height());
          });
        }
      }

      $(window).on("load", mobileViewUpdate);
      $(window).on("resize", mobileViewUpdate);

      mobileViewUpdate();
    });

  }
}
</script>

<style>
/* Style Here */
</style>
