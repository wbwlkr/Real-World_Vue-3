<template>
  <h1>Event Aie</h1>
  <div class="events">
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <EventCard v-for="event in events" :event="event" :key="event.id" />
  </div>
</template>

<script>
// @ is an alias to /src
import EventCard from "@/components/EventCard.vue";

export default {
  name: "Home",
  components: {
    EventCard
  },
  data() {
    return {
      events: [
        {
          id: 3444320,
          category: "plop category",
          title: "title plop",
          description: "description plop",
          location: "location plop",
          date: "April 1, 2022",
          time: "12:00",
          petsAllowed: true,
          organizer: "organizer plop"
        },
        {
          id: 3444321,
          category: "plop2 category",
          title: "title plop2",
          description: "description plop2",
          location: "location plop2",
          date: "April 1, 2022",
          time: "12:30",
          petsAllowed: true,
          organizer: "organizer plop2"
        },
        {
          id: 3444322,
          category: "plop3 category",
          title: "title plop3",
          description: "description plop3",
          location: "location plop3",
          date: "April 1, 2022",
          time: "13:30",
          petsAllowed: true,
          organizer: "organizer plop3"
        }
      ]
    };
  }
};
</script>

<style scoped>
.events {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>