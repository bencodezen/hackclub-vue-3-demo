<script>
export default {
  data: () => ({
    count: 10,
    color: '#222'
  })
}
</script>

<template>
  <h1 class="title" :style="`color: ${color}`">Test</h1>

  <input type="color" v-model="color" />

  <button type="button" @click="count++">count is: {{ count }}</button>
  <p class="description">
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<style>
.description,
.title {
  color: v-bind(color);
}
</style>
