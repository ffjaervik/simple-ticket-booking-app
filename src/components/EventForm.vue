<template>
    <div>
        <form>
          <label for="name">Name:</label>
          <input type="text" id="name" name="name" />
          <label for="email">Email:</label>
          <input type="email" id="email" name="email" />
        </form>

    </div>
</template>

<script>
    export default {
        name: "EventForm",
        props: {
        }
    }
</script>

<style scoped>

</style>