<template>
  <section v-for="resource in storedResources" :key="resource.id" class="w-3/5 mx-auto bg-white"
  >
    <div class="flex justify-between mx-auto w-5/6">
      <h3>{{ resource.header }}</h3>
      <button>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
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
    <div class="mx-auto w-5/6">
      <p>{{ resource.desc }}</p>
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
          desc: "Learn to google....",
        },
      ],
    };
  },
};
</script>