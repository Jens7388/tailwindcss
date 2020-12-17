<template>
  <div class="max-w-2xl m-auto py-10">
    <header class="flex justify-between px-5">
      <h3 class="text-gray-400 mt-2 font-semibold">REMEMBER ME</h3>
      <button class="px-4 py-2 rounded-md bg-blue-100 text-blue-700 hover:bg-blue-800 hover:text-white">+ Add</button>
    </header>
    <div class="flex flex-col ">
      <resources />
    </div>
      <button class="flex justify-center max-w-2x1 w-11/12 m-auto p-5 border-2 border-dashed border-gray-300 text-gray-400">Add resource</button>  
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