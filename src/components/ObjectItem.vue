<template>
  <div v-bind="$attrs">
    <div class="grid-item">{{ index + 1 }}</div>
    <div class="grid-item">{{ object.name }}</div>
    <div class="grid-item">{{ object.objectType }}</div>
    <div class="grid-item">{{ object.massKg }}</div>
    <div class="grid-item">{{ object.radiusKm }}</div>
    <div class="grid-item">{{ object.densityGCm3 }}</div>
    <div class="grid-item">{{ object.temperatureK }}</div>
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
