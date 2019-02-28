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
  </header>
</template>

<script>
export default {
  name: 'Header',
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
  padding: 2em 32px
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