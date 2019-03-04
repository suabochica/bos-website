<template>
  <section id="services" class="services--grid">
    <h2 class="services__title">Servicios</h2>
    <div class="services__card">
      <h2>Análisis Estratégicos</h2>
      <ul>
        <li>Seguimiento de resultados</li>
        <li>Análisis de rendimientos y tendecias</li>
        <li>Evaluación y orientación de las capacidades</li>
      </ul>
    </div>
    <div class="services__card">
      <h2>Entrenamientos Alternativos</h2>
      <ul>
        <li>Entrenamiento en realidad virtual</li>
        <li>In Situ</li>
      </ul>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Services',
}
</script>

<style>
.services--grid {
  background-color: var(--black);
  color: var(--white);
  display: grid;
  grid-template-columns: repeat(2, 1fr [card__col__item]);
  grid-template-rows: 96px repeat(1, 400px [card__row__item]);
  grid-gap: 8px;
  padding: 40px 0;
}

.services__title {
  text-align: center;
  grid-column: 1 / 4;
  grid-row: 1 / 2;
}

.services__card {
  align-self: center;
  justify-self: center;
  text-align: center;
  padding: 0 24px 16px;
}

.services__card h2 {
  font-family: 'Fira Sans', sans-serif;
  font-style: italic;
  font-weight: bold;
  text-transform: uppercase;
  padding-bottom: 16px;
  word-break: break-all;
}

.services__card ul {
  list-style: square inside;
  text-align: left;
}

.services__card li {
  display: list-item;
  font-family: 'Fira Sans', sans-serif;
  font-size: 16px;
  line-height: 1.6;
  padding-bottom: 16px;
}

</style>
