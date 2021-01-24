<template>
  <div class="container">
    <ul>
      <ObjectItem
          v-for="(object, i) of objects" :key="object.id"
          v-bind:object="object"
          v-bind:index="i"
      />
    </ul>
  </div>
</template>

<script>
import ObjectItem from '@/components/ObjectItem'
export default {
  props: ['objects'],
  components: {
    ObjectItem
  }
}
</script>

<style>
.container {
  width: 100%;
  max-width: 1200px;
  margin: 0px auto;
}
ul {
  list-style: none;
  padding: 0;
}
</style>
