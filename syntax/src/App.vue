<template>
  <h1>Hello world</h1>
  <h2>user: {{ user }}</h2>
  <hr />
  <Races />
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'
import RacesPony from '@/components/Races.vue'

export default defineComponent({
  name: 'App',
  components: {
    Races: RacesPony
  },
  setup() {
    const user = ref({
      id: 1,
      name: 'Dinh'
    })

    return { user }
  }
})
</script>
