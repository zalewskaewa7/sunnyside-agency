<script setup>
import Footer from './components/Footer.vue';
import Header from './components/Header.vue'
import Content from './components/content/Content.vue'

</script>

<template>
  <header>
    <Header />
    
  </header>

  <main>
<Content />
  </main>
  <footer>
    <Footer />
  </footer>
</template>

<style lang="scss" scoped>

@font-face {
    font-family: Barlow;
    src: url('./assets/fonts/Barlow/Barlow-Black.ttf');
}
@font-face {
    font-family: Fraunces;
    src: url('./assets/fonts/Fraunces/static/Fraunces_9pt-Black.ttf');
}
@font-face {
    font-family: BarlowThin;
    src: url('./assets/fonts/Barlow/Barlow-SemiBold.ttf');
}
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
  padding:0;
  font-weight: normal;
}
#app {
  max-width: 1280px;
  margin: 0 auto;
  padding: 0;
  font-family: "Barlow";
  font-weight: 600;
}
body {
  margin: 0;
  padding:0;
  min-height: 100vh;
}
header{
  margin: 0;
  padding: 0;
}
footer{
  display: flex;
  justify-content: center;
    background-color: hsl(168, 34%, 41%, .6);
}
</style>
