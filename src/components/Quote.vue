<template>
  <section class="quote">
    <div class="quote__square"></div>
    <h1 class="quote__header">¡Forjando grandeza!</h1>
    <div class="quote__container">
      <p
        class="quote__paragraph"
      >Prueba nuesta aplicación de android para registrar los resultados de un combate de esgrima</p>
      <a
        class="button"
        href="http://bos.com.co/apk/fencing_fast_stats_v1.0.apk"
        download="fencing_fast_stats_v1.0"
      >
        <i class="fa fa-download"></i>Descargar
      </a>
    </div>
    <div class="quote__square"></div>
  </section>
</template>

<script>
export default {
  name: "Quote"
};
</script>

<style>
.quote {
  padding: 56px 0 64px;
}

.quote__square {
  background-image: url("../assets/quote_square.png");
  background-repeat: no-repeat;
  background-position: center;
  height: 24px;
  margin: 0 auto;
  position: relative;
  width: 24px;
  z-index: 2;
}

.quote__header {
  color: var(--back);
  font-family: "Fira Sans", sans-serif;
  font-size: 64px;
  font-style: italic;
  font-weight: 900;
  text-transform: uppercase;

  margin: 80px 0;
}

.quote__container {
  display: flex;
  justify-content: center;
  flex-direction: column;
  height: 184px;
}

.quote__paragraph {
  font-weight: bold;
}

.button {
  align-self: center;
  background-color: var(--gold);
  border: none;
  color: var(--black);
  cursor: pointer;
  font-family: "Fira Sans", sans-serif;
  font-weight: bold;
  text-decoration: none;
  padding: 12px 30px;
  margin: 24px;
  width: 200px;
}

.button i {
  padding-right: 8px;
}

.button:hover {
  background-color: var(--ocre);
}
</style>
