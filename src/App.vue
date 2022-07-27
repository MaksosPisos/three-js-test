<template>
  <Renderer ref="renderer" resize="window" orbit-ctrl>
    <Camera :position="{ z: 10 }" />
    <Scene background="#fff">
      <AmbientLight color="#aaaaaa" />
      <PointLight :position="{ y: 100, z: 0 }" />
      <GltfModel ref="box" src="../public/adamHead.gltf" />
    </Scene>
  </Renderer>
</template>

<script>
export default {
  mounted() {
    // const renderer = this.$refs.renderer;
    // const box = this.$refs.box.mesh;
    // renderer.onBeforeRender(() => {
    //   box.rotation.x += 0.01;
    // });
  },
};
</script>