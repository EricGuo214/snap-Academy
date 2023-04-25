<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>Unofficial site with new design</h3>

    <hr>
    
    <p>Current time: {{ currentTime }}</p>

    <p>Store status: {{ openOrClosed }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentDateTime: new Date(),
    };
  },
  mounted() {
    setInterval(() => {
      this.currentDateTime = new Date();
    }, 1000);
  },
  computed: {
    currentTime() {
      return this.currentDateTime.toLocaleTimeString();
    },
    openOrClosed() {
      var hour = this.currentDateTime.getHours();
      return 10 <= hour && hour < 20 ? "Open" : "Closed";
    },
  },
};
</script>


<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
