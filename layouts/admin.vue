<template>
  <div>
    <NavBar />
    <nuxt />
  </div>
</template>

<script>
import NavBar from "@/components/NavBarAdmin.vue";
export default {
  name: "admin",
  components: {
    NavBar
  }
};
</script>

<style scoped></style>
