<template>
    <div>
  <b-navbar toggleable="lg" type="light" variant="light">
    <b-container>
    <b-navbar-brand href="#">Kuliner</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <router-link class="nav-link" to = "/">Home</router-link>
        <router-link class="nav-link" to = "/foods">Foods</router-link>
      </b-navbar-nav>

      <b-navbar-nav class="ml-auto">
        <router-link class="nav-link" to = "/keranjang">
        Keranjang 
        <b-icon-bag></b-icon-bag>
        <span class="badge badge-success ml-2">0</span>
        </router-link>
      </b-navbar-nav>
    </b-collapse>
    </b-container>
  </b-navbar>
</div>
</template>

<script>
export default {
  name: 'Navbar',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
