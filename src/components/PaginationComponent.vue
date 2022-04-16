<template>
  <section class="mt-5 pt-5">
    <nav aria-label="Page navigation example">
      <ul class="pagination pagination-lg justify-content-center">
        <li class="page-item disabled">
          <router-link class="page-link border-0 bg-transparent" to="#" tabindex="-1" aria-disabled="true">
            Previous
          </router-link>
        </li>
        <li class="page-item">
          <router-link class="page-link border-0 bg-transparent" to="#">
            1
          </router-link>
        </li>
        <li class="page-item">
          <router-link class="page-link border-0 bg-transparent" to="#">
            2
          </router-link>
        </li>
        <li class="page-item">
          <router-link class="page-link border-0 bg-transparent" to="#">
            3
          </router-link>
        </li>
        <li class="page-item">
          <router-link class="page-link border-0 bg-transparent" to="#">
            Next
          </router-link>
        </li>
      </ul>
    </nav>
  </section>
</template>

<script>
export default {
  name: "PaginationComponent",
}
</script>