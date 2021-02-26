<template>
  <h2>Coche</h2>
  <p>Marca: {{ brand }}</p>
  <p>Modelo: {{ model }}</p>
  <p>Color: {{ color[1] }}</p>
  <p>Precio: {{ price }}</p>
  <p>Potencia: {{ power }} CV</p>
  {{mensaje.title}} - {{mensaje.text}}
</template>

<script>
export default {
/*Options API*/
  // data() {
  //   return {
  //     brand: "Audi",
  //     model: "A4",
  //     color: ["Azul", "Rojo", "Verde"],
  //     price: 38000,
  //     power: 180,
  //     mensaje: {
  //       title: "Hola mundo",
  //       text: "Adiós",
  //     }
  //   };
  // },

/*Composition API*/
  setup() {
    const brand = "Audi";
    const model = "A4";
    const color = ["Azul","Morado", "Marrón"];
    const price = 45000;
    const power = 240;
    const mensaje = {
      title: "Estoy bien",
      text: "Welcome",
    }
    return {
      brand,
      model,
      color,
      price,
      power,
      mensaje,
    }
  },
};
</script>

<style></style>
