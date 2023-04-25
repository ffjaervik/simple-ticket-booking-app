<template>
  <li>Choose your city</li>
  <p>{{ allData.city }}</p>
  <li>Choose your event</li>
  <div v-for="event in allData.events" :key="event.id">
    <p>{{ event.name }}</p>
  </div>
  <li>Register</li>
</template>

<script>
  export default {
    name: "CityDetail",
    props: {
      allData: Object,
    },
  };
</script>

<style scoped></style>
