<script setup>
import Vheader from "./components/Vheader.vue";
import Vpromo from "./components/Vpromo.vue";
import Vclassroom from "./components/Vclassroom.vue";
import Vdistance from "./components/Vdistance.vue";
import Vfooter from "./components/Vfooter.vue";
import Vlessons from "./components/Vlessons.vue";
import Vopportunities from "./components/Vopportunities.vue";
import VshaduleWork from "./components/VschaduleWork.vue";

  components: { Vfooter }
  components: { Vdistance }
  components: { VshaduleWork }
  components: { Vopportunities }
  components: { Vlessons }
  components: { Vclassroom }
  components: { Vpromo }
  components: { Vheader }

</script>

<template>
    <vheader/>
    <main>
        <vpromo/>
        <vclassroom/>
        <vlessons/>
        <vopportunities/>
        <vshaduleWork/>
        <vdistance/>
    </main>
    <vfooter/>
</template>

<style scoped>

</style>
