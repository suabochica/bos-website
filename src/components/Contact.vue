<template>
  <section id="contact" class="contact--grid" method="post">
    <h2 class="contact__title">Contacto</h2>
    <form class="contact__form" name="contact_form" @submit.prevent="handleSubmit">
      <label for="name">Nombre</label>
      <input type="text" name="name" v-model="contact.name">
      <label for="email">Correo Electrónico</label>
      <input type="text" name="email" v-model="contact.email">
      <label for="message">Mensaje</label>
      <textarea name="message" id="" cols="30" rows="10" v-model="contact.message"></textarea>
      <input type="submit" id="submit" value="ENVIAR" @click="handleSubmit">
    </form>
    <aside class="contact_address">
      <h3>Información de Contacto</h3>
      <p><b>Teléfono:</b> (+571) 311 809 5133</p>
      <p><b>Correo Electrónico:</b> bossportsco@gmail.com</p>
    </aside>
  </section>
</template>

<script>
export default {
  name: 'Contact',
  data() {
    return {
      contact: {
        name: '',
        email: '',
        message: '',
      }
    }
  },

  methods: {
    handleSubmit: function() {
      return `hola`
    }
  }
}
</script>

<style>
.contact--grid {
  background-color: var(--gainsboro);
  color: var(--black);

  display: grid;
  grid-template-columns: repeat(2, 1fr [card__col__item]);
  grid-template-rows: 96px repeat(1, 360px [card__row__item]);
  grid-gap: 8px;

  padding: 40px 0;
}

.contact__title {
  text-align: center;

  grid-column: 1 / 4;
  grid-row: 1 / 2;
}

.contact__form {
  justify-self: center;
  padding: 0 64px 16px;
}

.contact__form label,
.contact__form textarea,
.contact__form input[type="text"],
.contact__form input[type="submit"] {
  display: inline-block;

  width: 100%;
}

.contact__form label {
  font-family: 'Fira Sans', sans-serif;
  font-weight: bold;
  text-transform: uppercase;

  padding: 8px 0 2px;
}

.contact__form textarea,
.contact__form input[type="text"] {
  background-color: var(--white);
  border: 1px solid var(--gray-dim);

  font-family: 'Fira Sans', sans-serif;

  padding: 6px 4px;
}

.contact__form input[type="submit"] {
  background-color: var(--salmon);
  border: 1px solid var(--scarlet);
  color: var(--white);

  font-family: 'Fira Sans', sans-serif;

  padding: 6px 4px;
  margin-top: 16px;
}
</style>
