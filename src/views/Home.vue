<template>
  <div>
    <b-row>
      <div class="col-lg mb-2">
        <h3>Home
          <small class="text-muted"> | Welcome</small>
        </h3>
        <router-link to="product/create">Novo</router-link>
      </div>
    </b-row>
  </div>
</template>

<script>
  import {BRow} from 'bootstrap-vue'
  export default {
    name: "Home",
    components: {
      BRow
    }
  }
</script>

<style scoped>

</style>