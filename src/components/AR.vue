<template>
  <a-scene embedded arjs>
    <a-marker preset="hiro">
      <a-entity
          position="0 0 0"
          scale="0.05 0.05 0.05"
          gltf-model='../assets/scene.gltf'
      ></a-entity>
    </a-marker>
    <a-entity camera></a-entity>
  </a-scene>

</template>

<script>

import "@ar-js-org/ar.js";

export default {
  name: "AR",
  methods: {
    markerFoundEvent(e) {
        console.log(e)
    }
  }
}
</script>

<style scoped>

</style>