<template>
  <li>
    {{ index + 1 }}. {{ object.name }} {{ object.objectType }}
  </li>
</template>

<script>
export default {
  props: {
    object: {
      type: Object,
      required: true
    },
    index: Number
  }
}
</script>

<style>
li {
  margin: 30px auto;
}
</style>
