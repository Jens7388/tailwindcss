<template>
  <div>
    <header class="flex justify-around">
      <h3 class="text-gray-500 font-semibold">Remember me</h3>
      <button>+ Add</button>
    </header>
    <div class="flex flex-col ">
      <resources />
    </div>
      <button>Add resource</button>
    
  </div>
</template>

<script>
import Resources from "./components/Resources.vue";

export default {
  name: "App",
  components: {
    Resources,
  },
};
</script>

<style>
</style>
