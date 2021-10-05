<template>
  <div class="about">
    <Sidebar></Sidebar>
    <div class="content" id="content">
    <h1>This is an about page</h1>
    <button class="btn btn-danger">Ahmad</button>
  </div></div>
</template>
<script>
import Sidebar from "@/components/sidebar.vue";
export default {
  name: "About",
   components: {
    Sidebar,
  },
}
</script>
<style scoped>

</style>