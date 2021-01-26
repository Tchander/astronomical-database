<template>
  <select v-model="filterByType" @click="$emit('filter-by-type', filterByType)">
    <option value="all">All Objects</option>
    <option value="stars">Stars</option>
    <option value="planets">Planets</option>
    <option value="dwarf-planets">Dwarf Planets</option>
    <option value="satellites">Satellites</option>
    <option value="asteroids">Asteroids</option>
  </select>

</template>

<script>
export default {
  data() {
    return {
      filterByType: 'all'
    }
  }
}
</script>

