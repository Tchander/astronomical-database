<template>
  <div>
    <router-link to="/all-objects">All Objects</router-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      allObjects: [
        {
          id: 1, name: 'Sun', objectType: 'Star', massKg: 1.9885e+30, radiusKm: 695700, densityGCm3: 1.408,
          rotationPeriodDays: 25.05, temperatureK: 5772, knownPlanets: 8, typeOfStar: 'G2V',
          descriptionOfType: 'Yellow Dwarf', age: 4.6e+9, distanceToTheSun: 0, rightAscension: 0, declination: 0
        },
        {
          id: 2, name: 'Jupiter', objectType: 'Planet', massKg: 1.8982e+27, radiusKm: 69911, densityGCm3: 1.326,
          rotationPeriodDays: 0.41375, temperatureK: 139, knownSatellites: 79, orbitalParent: 'Sun',
          aphelionKm: 816.62e+6, perihelionKm: 740.52e+6, semiMajorAxisKm: 778.57e+6, orbitalPeriodDays: 4332.59,
          eccentricity: 0.0489, inclination: 1.303, argumentOfPerihelion: 273.867, longitudeOfAscendingNode: 100.464,
          meanAnomaly: 20.020, albedo: 0.538
        },
        {
          id: 3, name: 'Earth', objectType: 'Planet', massKg: 5.97237e+24, radiusKm: 6371, densityGCm3: 5.514,
          rotationPeriodDays: 0.99726968, temperatureK: 287.16, knownSatellites: 1, orbitalParent: 'Sun',
          aphelionKm: 152100000, perihelionKm: 147095000, semiMajorAxisKm: 149598023, orbitalPeriodDays: 365.256363004,
          eccentricity: 0.0167086, inclination: 0.00005, argumentOfPerihelion: 114.20783,
          longitudeOfAscendingNode: '-11.26064', meanAnomaly: 358.617, albedo: 0.367
        },
        {
          id: 4, name: 'Moon', objectType: 'Satellite', massKg: 7.342e+22, radiusKm: 1737.4, densityGCm3: 3.344,
          rotationPeriodDays: 27.321661, temperatureK: 250, knownSatellites: 0, orbitalParent: 'Earth',
          aphelionKm: 405400, perihelionKm: 362600, semiMajorAxisKm: 384399, orbitalPeriodDays: 27.321661,
          eccentricity: 0.0549, inclination: 5.145, argumentOfPerihelion: 'unknown',
          longitudeOfAscendingNode: 'unknown', meanAnomaly: 'unknown', albedo: 0.136
        },
        {
          id: 5, name: 'Ganymede', objectType: 'Satellite', massKg: 1.4819e+23, radiusKm: 2634.1, densityGCm3: 1.936,
          rotationPeriodDays: 7.15455296, temperatureK: 110, knownSatellites: 0, orbitalParent: 'Jupiter',
          aphelionKm: 1071600, perihelionKm: 1069200, semiMajorAxisKm: 1070400, orbitalPeriodDays: 7.15455296,
          eccentricity: 0.0013, inclination: 0.20, argumentOfPerihelion: 'unknown', longitudeOfAscendingNode: 'unknown',
          meanAnomaly: 'unknown', albedo: 0.43
        }
      ]
    }
  }
}
</script>
