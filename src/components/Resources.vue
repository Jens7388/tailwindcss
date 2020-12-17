<template>
  <section v-for="resource in storedResources" :key="resource.id" class="mb-5 h-20 w-4/5 m-auto bg-white">
    <div class="mt-3 flex justify-between m-auto w-11/12">
      <h3 class="font-medium">{{ resource.header }}</h3>
      <button>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          stroke="lightgray"
          width="24"
          height="24"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M10 14l2-2m0 0l2-2m-2 2l-2-2m2 2l2 2m7-2a9 9 0 11-18 0 9 9 0 0118 0z"
          />
        </svg>
      </button>
    </div>
    <div class="m-auto w-11/12">
      <p class="pt-1 text-gray-500">{{ resource.desc }}</p>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      storedResources: [
        {
          id: "official-guide",
          header: "Official guide",
          desc: "The official Vue.js documentation.",
        },
        {
          id: "google",
          header: "Google",
          desc: "Learn to google...",
        },
      ],
    };
  },
};
</script>