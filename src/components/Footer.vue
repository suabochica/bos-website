<template>
  <footer class="footer footer--flex">
    <nav class="footer__nav">
      <ul class="footer__list">
        <li><a class="footer__anchor" href="#principles">Principios</a></li>
        <li><a class="footer__anchor" href="#services">Servicios</a></li>
        <li><a class="footer__anchor" href="#contact">Conacto</a></li>
      </ul>
    </nav>
    <img class="footer__image" alt="Bos logo" src="../assets/bos_pictogram.png">
    <p class="footer__rigths">2019 Bos Company.</p>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
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

.footer {
  background-color: var(--black);
  color: var(--white);
  padding: 2em 0
}

.footer--flex {
  align-items: center;
  display: flex;
  justify-content: space-around;
}

.footer__rigths {
  margin-left: 10px;
}

.footer__image {
  width: 80px;
  height: 80px;

  margin-right: 80px;
}

.footer__anchor {
  color: var(--white);

  font-family: 'Fira Sans', serif;
  font-size: 16px;
}

</style>