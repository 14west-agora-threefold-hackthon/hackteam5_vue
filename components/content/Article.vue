<template>
  <v-container id="about" tag="section">
    <base-subheading>PUB_CODE_NAME</base-subheading>
    <p>
      {{ $store.state.title }}
    </p>
  </v-container>
</template>

<script>
import axios from 'axios'
export default {
  name: 'Article',
  async fetch({ store, params }) {
    const { data } = await axios.get(
      'https://jsonplaceholder.typicode.com/todos/1'
    )
    console.log('Returned Data ', data)
    store.commit('setStars', data)
  }
}
</script>
