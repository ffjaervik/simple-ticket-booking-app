<template>
  <div id="app">
    <h1>Book your tickets here in a few simple steps:
      <ol>
        <li>Choose your city</li>
        <li>Choose your event</li>
        <li>Register</li>
        <li>Relax</li>
      </ol>
    </h1>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {
  },
  data(){
    return {
      city: "London",
      events: [
        {name: "The Lion King", date: "2019-07-01", time: "19:00", price: 50, registeredUser: []},
        {name: "Wicked", date: "2019-07-02", time: "19:00", price: 39, registeredUser: []},
        {name: "The Phantom of the Opera", date: "2019-07-03", time: "19:00", price: 40, registeredUser: []},
        {name: "The Book of Mormon", date: "2019-07-04", time: "19:00", price: 29, registeredUser: []},
        {name: "Hamilton", date: "2019-07-05", time: "19:00", price: 34, registeredUser: []},
      ],
      

    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;

}
</style>
