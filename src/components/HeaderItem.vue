<template>
  <div>
    <div class="grid-item-header">№</div>
    <div class="grid-item-header">Name</div>
    <div class="grid-item-header">Type</div>
    <div class="grid-item-header">Mass(kg)</div>
    <div class="grid-item-header">Radius(km)</div>
    <div class="grid-item-header">Density(g/cm^3)</div>
    <div class="grid-item-header">Temperature(K)</div>
  </div>
</template>

<style>
.grid-item-header{
  display: flex;
  align-items: center;
  justify-content: center;
  border-left: 1px solid #fff;
  border-bottom: 1px solid #fff;
  border-top: 1px solid #fff;
  font-size: 18px;
  font-weight: 700;
  color: #fff;
}
.grid-item-header:last-child{
  border-right: 1px solid #fff;
}
</style>
