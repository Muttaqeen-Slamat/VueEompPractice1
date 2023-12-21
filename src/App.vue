<template>
  <main class="container-fluid">
    <NavBar/>
    <Footer/>
    <router-view/>
  </main>
</template>

<script >
import NavBar from './components/NavBar.vue';
import Footer from './components/Footer.vue';
export default{
    component: {
        NavBar,
        Footer
    },
    components: { NavBar }
}
</script>

<style src="@/assets/css/styles.css">

</style>