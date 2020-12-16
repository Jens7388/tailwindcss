<template>
    <section v-for="resource in storedResources" :key="resource.id">
        <h3> {{ resource.header }} </h3>
        <p>  {{ resource.desc }}</p>
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