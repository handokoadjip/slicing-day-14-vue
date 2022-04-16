<template>
  <section class="mb-5">
    <div class="container-fluid">
      <div class="row min-vh-100 mb-5" v-for="(list, index) in lists" :key="index" :id="list.title">
        <div
          :class="`col-lg-6 mb-5 mb-lg-0 min-vh-50 ${list.image} ${index % 2 === 0 ? 'order-0' : 'order-0 order-lg-1'}`">
        </div>
        <div :class="`col-lg-6 d-flex align-items-lg-end ${index % 2 === 0 ? 'order-1' : 'order-1 order-lg-0'}`">
          <div class="wrapper ms-5">
            <h2 class="display-5 text-border-bottom-center text-capitalize fw-bold">
              {{list.title}}
            </h2>
            <p class="leading-loose mb-5">{{list.description}}</p>
            <Link class="link d-block mb-8rem fw-bold" :to="list.href">
            View Pages
            <i class="ms-3 fas fa-arrow-right"></i>
            </Link>
            <p class="text-fade-black-1 fw-bold">{{list.subtitle}}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ContentComponent",
  data() {
    return {
      lists: [
        {
          image: "bg-image-1",
          title: "Minimalist Apartment",
          description: "Lorem ipsum dolor sit.",
          href: "#",
          subtitle: "lorem",
        },
        {
          image: "bg-image-2",
          title: "Jx Create",
          description: "Lorem ipsum dolor sit.",
          href: "#",
          subtitle: "lorem",
        },
        {
          image: "bg-image-3",
          title: "Pelitre Hall",
          description: "Lorem ipsum dolor sit.",
          href: "#",
          subtitle: "lorem",
        },
        {
          image: "bg-image-4",
          title: "Mave House",
          description: "Lorem ipsum dolor sit.",
          href: "#",
          subtitle: "lorem",
        },
      ]
    }
  }
}
</script>