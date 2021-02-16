<template>
  <div class="about">
    <h1>page{{ id }}</h1>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: 1
    }
  },
  created() {
    this.fetchData();
  },

  methods: {
    fetchData () {
      this.id = this.$route.query.id
    }
  }
}
</script>