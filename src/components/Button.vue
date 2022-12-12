<template>
  <button
    type="button"
    v-on:click="movie.quantity -= 1"
    :disabled="movie.quantity <= 0"
  >
    -
  </button>
  {{ movie.quantity }}
  <button
    type="button"
    v-on:click="movie.quantity += 1"
    :disabled="movie.quantity >= movie.available"
  >
    +
  </button>
  -->
</template>

<style lang = "scss" scoped>
@import "../styles/_variables.scss";
button {
  background: $color2;
  border: 1px solid transparent;
  cursor: pointer;
  padding: 5px 10px;
  transition: border-color 0.15;
}
button:hover {
  border-color: $color2;
}
button[disabled] {
  opacity: 0.5;
}
</style>