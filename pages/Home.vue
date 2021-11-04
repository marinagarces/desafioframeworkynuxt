<template>
  <div>
    <v-row justify="center" class="mt-12">
      <v-col cols="11">
        <v-row>
          <v-col v-for="personaje in personajes" :key="personaje.id" lg="4" xl="4" md="4" sm="3" cols="12">
            <Personajes :personaje="personaje" />
          </v-col>
        </v-row>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import Personajes from '../components/Personajes'

export default {
  name: 'Home',
  components: {
    Personajes,
  },
  computed: {
    personajes() {
      return this.$store.getters.getPersonajes
    },
  },
}
</script>
