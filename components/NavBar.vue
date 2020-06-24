<template>
  <div>
    <b-navbar toggleable="lg" type="dark" variant="danger">
      <b-container>
        <b-navbar-brand href="/">
          <nuxt-link to="/" class="nav-link brand-title"
            >Mon App NuxtJS</nuxt-link
          >
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav class="ml-auto">
            <li class="nav-item">
              <nuxt-link to="/login" class="nav-link">Login</nuxt-link>
            </li>
          </b-navbar-nav>
        </b-collapse>
      </b-container>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "NavBar"
};
</script>

<style scoped>
a.brand-title {
  color: #ffffff !important;
}
a.brand-title:hover {
  color: #ffffff !important;
}
</style>
