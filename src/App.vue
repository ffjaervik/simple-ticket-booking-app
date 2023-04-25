<template>
  <div id="app">
    <h1>
      Book your tickets here in a few simple steps:
      <ol>
        <CityDetail :allData="allData" />
        <EventForm />
      </ol>
    </h1>
  </div>
</template>

<script>
  import CityDetail from "./components/CityDetail.vue";
  import EventForm from "./components/EventForm.vue";

  export default {
    name: "App",
    components: { CityDetail, EventForm },
    data() {
      return {
        allData: {
          city: "London",
          events: [
            {
              id: 1,
              name: "The Lion King",
              date: "2019-07-01",
              time: "19:00",
              price: 50,
              registeredUser: [],
            },
            {
              id: 2,
              name: "Wicked",
              date: "2019-07-02",
              time: "19:00",
              price: 39,
              registeredUser: [],
            },
            {
              id: 3,
              name: "The Phantom of the Opera",
              date: "2019-07-03",
              time: "19:00",
              price: 40,
              registeredUser: [],
            },
            {
              id: 4,
              name: "The Book of Mormon",
              date: "2019-07-04",
              time: "19:00",
              price: 29,
              registeredUser: [],
            },
            {
              name: "Hamilton",
              date: "2019-07-05",
              time: "19:00",
              price: 34,
              registeredUser: [],
            },
          ],
        },
      };
    },
    // methods: {
    // async getEvents() {
    // const data = await this.events
    // return data;

    // },
    // },
    // mounted() {
    //   this.getEvents();
    // },
  };
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
  }
</style>
