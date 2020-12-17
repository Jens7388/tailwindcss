<template>
  <div class="pb-10">
    <header class="flex justify-between w-4/5 m-auto py-10">
      <h3 class="text-gray-400 mt-2 font-semibold">REMEMBER ME</h3>
      <button class="h-9 px-4 rounded-md bg-blue-100 text-blue-700">+ Add</button>
    </header>
    <div class="flex flex-col ">
      <resources />
    </div>
      <button class="flex justify-center w-4/5 m-auto py-5 border-2 border-dashed border-gray-300 text-gray-400">Add resource</button>  
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