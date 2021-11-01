<template>
  <div>
    <h1>Mountains</h1>
    <LazyMountainsList v-if="show" />
    <button v-if="!show" @click="show = true">Show List</button>
    <Documents />
  </div>
</template>

<script>
import Documents from '../components/documents.vue'
import LazyMountainsList from './LazyMountainsList.vue'
export default {
  components: {
    LazyMountainsList,
    Documents,
  },
  data() {
    return {
      show: false,
    }
  },
}
</script>

<style scoped>
  *{
    font-family: monospace;
  }
</style>
