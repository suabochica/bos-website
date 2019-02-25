<template>
  <section class="principles--grid">
    <div class="principles__card">
      <h2>Admira la grandeza</h2>
      <p>La grandeza inspira a los demas. La grandeza no es buscar reconocimientos ni pensar que se és superior a los demas, es realizar las cosas de una forma tan excelsa que toca la vida de los demas</p>
    </div>
    <div class="principles__card">
      <h2>Máximo Esfuerzo</h2>
      <p>Es necesarion entregarse al máximo en todas la actividades y acciones que se realicen. Dar siempre mas del 100% sin fijarse a los demas. No damos excusas, vamos al frente con toda la actitud</p>
    </div>
    <div class="principles__card">
      <h2>Siempre Ataca</h2>
      <p>Entre hace algo y no hacer nada, es mejor siempre hacer algo, No hay que darse por vencido, rendirse no es una opción y por eso siempre intenta hacer las cosas</p>
    </div>
    <div class="principles__card">
      <h2>Abrazar la Dificultad</h2>
      <p>De la dificultad surge la grandeza. Nada extraordinario se logra con facilidad. La dificultad es nuestra mejor aliada, por es hay que buscarla. Atravesar la dificultad nos fortalece, nos enseña y nos da felicidad</p>
    </div>
    <div class="principles__card">
      <h2>Aprender del Fracaso</h2>
      <p>E; fracasp es parte del proceso y es un resultado al que todos los  mortales estamos expuestos. Todos los días escuchamos historia de éxito y fracaso y siempre se concluye que el fracaso es la madre de todos los éxitos</p>
    </div>
    <div class="principles__card">
      <h2>Vive el Momento</h2>
      <p>La mortalidad nos hace entender que el tiempo se agota, que cada segundo vale oro y por eso hay que aprovecharlo al máximo. Solo se vive una vez</p>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Principles',
}
</script>

<style>
.principles--grid {
  background-color: var(--ocre);
  display: grid;
  grid-template-columns: repeat(3, 1fr [card__col__item]);
  grid-template-rows: repeat(2, 200px [card__row__item]);
  grid-gap: 8px;
  padding: 40px 0;
}

.principles__card {
  align-self: center;
  justify-self: center;
  text-align: center;
  padding: 0 24px;
}

.principles__card h2{
  font-family: 'Fira Sans', sans-serif;
  font-style: italic;
  font-weight: bold;
  text-transform: uppercase;
  padding-bottom: 16px;
}

</style>
