<template>
  <div class="container">
    <div class="row">
      <h2 class="display-2">About</h2>

    </div>
    <div class="row" v-if="about">
      <p class="lead" v-for="title in about" :key="title">
        {{ title }}
      </p>   
     </div>

  </div>
</template>
<script>
// @ is an alias to /src


export default {
  computed: {
    about(){
      return this.$store.state.about
    }
  },
  mounted(){
    this.$store.dispatch('fetchAbout')
  }
}
</script>