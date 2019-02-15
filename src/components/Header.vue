<template>
  <div id="header">
      <nav class="header__menu">
        <img alt="Bos logo" src="../assets/logo.png">
        <ul class="header__links">
            <li><a href="#principles">Principios</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Conacto</a></li>
        </ul>
      </nav>

  </div>
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
a {
  color: #42b983;
}

.header__menu {
    align-items: center;
    display: flex;
    justify-content: flex-end;
}

.header__links {
    flex-grow: 1;
    padding-left: 50%;
}

</style>