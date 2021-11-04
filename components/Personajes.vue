<template>
  <div>
    <v-card class="mx-auto" max-width="100%">
      <v-img class="white--text align-end" :src="personaje.imagen">
        <v-card-title> {{ personaje.nombre }} </v-card-title>
      </v-img>
    </v-card>
  </div>
</template>

<script>
export default {
  props: {
    personaje: Object,
  },
};
</script>

<style>
</style>