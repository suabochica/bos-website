<template>
  <section class="principles--grid">
    <div class="principles__card">Card 1</div>
    <div class="principles__card">Card 2</div>
    <div class="principles__card">Card 3</div>
    <div class="principles__card">Card 4</div>
    <div class="principles__card">Card 5</div>
    <div class="principles__card">Card 6</div>
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
}

.principles__card {
  background-color: var(--aqua);
  justify-self: center;
  align-self: center;
}

</style>
