<template>
  <div>
    <the-personal-data />    
    <the-about />
    <the-skills />
    
  </div>
</template>

<script>
import ThePersonalData from "../src/components/ThePersonalData.vue";
import TheAbout from "../src/components/TheAbout.vue";
import TheSkills from "../src/components/TheSkills.vue";
export default {
  name: 'App',
  components: {
    ThePersonalData,
    TheAbout,
    TheSkills,
    
  }
}
</script>

<style>
*{
  margin: 0px;
  padding: 0px;

}
</style>
