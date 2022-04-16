<template>
  <ContentComponent />
  <PaginationComponent />
</template>

<script>
import ContentComponent from "@/components/ContentComponent.vue";
import PaginationComponent from "@/components/PaginationComponent.vue";

export default {
  name: "HomePage",
    components: {
    ContentComponent,
    PaginationComponent,
  },
  mounted() {
    document.title = "Nikita Prokopiev | Projects"
  }
}
</script>
