<template>
    <section class="quote">
        <div class="quote__square"></div>
        <h1 class="quote__header">¡Encuentra tu propia grandeza! <br/> Nosotros te apoyamos. </h1>
        <div class="quote__square"></div>
    </section>
</template>

<script>
export default {
  name: 'Quote',
}
</script>

<style>
.quote {
  text-align: center;
  margin: 32px 0  16px;
}

.quote__square {
  background-image: url('../assets/quote_square.png');
  background-repeat: no-repeat;
  background-position: center;
  height: 24px;
  margin: 0 auto;
  position: relative;
  width: 24px;
  z-index: 2;
}

.quote__header {
  font-family: 'Fira Sans', sans-serif;
  font-size: 64px;
  font-style: italic;
  font-weight: 900;
  text-transform: uppercase;

  margin: 24px 0;
}
</style>
