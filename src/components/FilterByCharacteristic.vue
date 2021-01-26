<template>
  <select v-model="filterByCharacteristic" @click="$emit('filter-by-characteristics', filterByCharacteristic)">
    <option value="" disabled selected hidden>Characteristics</option>
    <option value="radius">Radius</option>
    <option value="mass">Mass</option>
    <option value="density">Density</option>
    <option value="temperature">Temperature</option>
  </select>

</template>

<script>
export default {
  data() {
    return {
      filterByCharacteristic: ''
    }
  }
}
</script>

