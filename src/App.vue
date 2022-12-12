

<template>
  <h2>peliculas</h2>
  <Form />
  <Button />
</template>

<script>
import Form from "./components/Form.vue";
import Button from "./components/Button.vue";
export default {
  name: "App",
  components: {
    Form: Form,
    Button: Button,
  },
};
</script>

<style lang ="scss">
@import "./styles/_variables.scss";
html,
body {
  background: $bg;
  color: $color;
  margin: 0;
  font-family: sans-serif;
}
h2 {
  border-bottom: 1px solid $color;
  padding-bottom: 10px;
}
</style>

