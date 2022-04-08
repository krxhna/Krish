<template>
  <div class="d">
    <Renderer resize="window" orbit-ctrl>
      <Camera :position="{ z: 10 }" />
      <Scene background="red">
        <PointLight :position="{ y: 50, z: 50 }" />
        <Box>
          <LambertMaterial />
        </Box>
      </Scene>
    </Renderer>
  </div>
</template>

<script lang="ts">
import { Box, Camera, LambertMaterial, PointLight, Renderer, Scene } from "troisjs";
import { defineComponent, ref } from "vue";
export default defineComponent({
  components: { Box, Camera, LambertMaterial, PointLight, Renderer, Scene },

  setup() {
    const renderer = ref(null);
    const box = ref(null);

    renderer?.value?.onBeforeRender(() => {
      box.value.mesh.rotation.x += 0.01;
    });


    return{renderer,box};
  },
});
</script>
