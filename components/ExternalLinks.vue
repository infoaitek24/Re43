<template>
  <div>
    <iframe v-if="links.imdb_id"
            :src="`https://vidsrc.xyz/embed/movie/${links.imdb_id}`"
            referrerpolicy="origin"
            width="640"
            height="480"
            allowfullscreen>
    </iframe>
  </div>
</template>

<script>
export default {
  props: {
    links: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
iframe {
  width: 100%; /* Responsive width */
  height: 500px; /* Fixed height, can adjust as needed */
  border: none; /* Remove default border */
  border-radius: 8px; /* Optional: rounded corners for the iframe */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* Optional: add shadow for better visual separation */
}
</style>
