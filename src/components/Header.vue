<template>
  <header class="header">
    <nav class="header__menu">
      <img class="header__image" alt="Bos logo" src="../assets/bos_imagotype_left.png">
      <ul class="header__list">
        <li><a class="header__anchor" href="#principles">Principios</a></li>
        <li><a class="header__anchor" href="#services">Servicios</a></li>
        <li><a class="header__anchor" href="#contact">Contacto</a></li>
      </ul>
    </nav>
    <Quote />
  </header>
</template>

<script>
import Quote from './Quote.vue'

export default {
  name: 'Header',
  components: {
    Quote
  }
}
</script>

<style>

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}


.header {
  text-align: center;
  position: relative;
  padding: 2em 32px
}

.header::before {
  content: "";
  background-image: url('../assets/quote_image_background.jpg');
  background-attachment: fixed;
  background-size: cover;
  background-position: 0%;

  filter: grayscale(1) opacity(.64);

  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;

  z-index: -1;
}

.header__menu {
  align-items: center;
  display: flex;
  justify-content: flex-end;
}

.header__list {
  flex-grow: 1;
  text-align: right;
}

.header__image {
  width: 180px;
  height: 80px;
}

.header__anchor {
  color: var(--black);

  font-size: 16px;
  font-family: 'Lato', sans-serif;
  font-weight: 900;
  letter-spacing: 2px;
  text-decoration: none;
  text-transform: uppercase;

  display: inline-flex;
  position: relative;
  z-index: 1;

  padding: 0 10px 5px;
}

.header__anchor::before {
  background: linear-gradient(to top, var(--gold) 25%, transparent 40%);
  content: "";

  height: 100%;
  width: 100%;

  bottom: 2px;
  left: 0;
  position: absolute;
  z-index: -1;

  transform: rotate(-2deg);
  transform-origin: left bottom;
  will-change: width;

  transition: width .1s ease-out;
}

.header__anchor:hover::before {
  width: 0;
  transition-duration: .15s;
}

</style>