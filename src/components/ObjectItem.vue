<template>
  <div v-bind="$attrs">
    <div class="grid-item">{{ index + 1 }}</div>
    <div v-for="key in keys" class="grid-item">{{ object[key] }}</div>
  </div>
</template>

<script>
export default {
  props: {
    object: {
      type: Object,
      required: true,
      default: () => ({})
    },
    index: Number
  },
  data() {
    return {
      keys: ['name', 'objectType', 'massKg', 'radiusKm', 'densityGCm3', 'temperatureK']
    }
  }
}
</script>

<style>
.grid-item{
  display: flex;
  align-items: center;
  justify-content: center;
  border-left: 1px solid #fff;
  border-bottom: 1px solid #fff;
  color: #fff;
}
.grid-item:last-child {
  border-right: 1px solid #fff;
}
</style>
