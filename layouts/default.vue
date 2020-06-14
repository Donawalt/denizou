<template>
  <div class="d-layout">
    <Header></Header>
    <main>
      <nuxt />
    </main>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from '@/components/Header'
import Footer from '@/components/Footer'

export default {
  components:{
    Header,
    Footer
  }
}
</script>

<style lang="scss">
$background-color: #232424;
$main-blue: #046BD9;
$main-pink: #FFAFAF;
html{
  background-color: $background-color;
}
body{
    background-color: $background-color;
    overflow-x: hidden;
}
</style>
