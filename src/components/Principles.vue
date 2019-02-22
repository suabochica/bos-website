<template>
  <section class="principles--grid">
    <div class="principles__card">
      <h2>Card 1</h2>
      <p>Lorem ipsum loren first paragraph</p>
    </div>
    <div class="principles__card">
      <h2>Card 2</h2>
      <p>Lorem ipsum loren second paragraph</p
    ></div>
    <div class="principles__card">
      <h2>Card 3</h2>
      <p>Lorem ipsum loren third paragraph</p>
    </div>
    <div class="principles__card">
      <h2>Card 4</h2>
      <p>Lorem ipsum loren fourth paragraph</p
    ></div>
    <div class="principles__card">
      <h2>Card 5</h2>
      <p>Lorem ipsum loren fifth paragraph</p>
    </div>
    <div class="principles__card">
      <h2>Card 6</h2>
      <p>Lorem ipsum loren sixth paragraph</p>
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
}

.principles__card {
  align-self: center;
  justify-self: center;
}

</style>
