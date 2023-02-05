<template>
  <div class="app">
    <VmainWrapper></VmainWrapper>
  </div>
</template>

<script>
import VmainWrapper from '@/components/v-main.vue'
export default {
  name: 'app',
  components: {
    VmainWrapper
  },
}
</script>

<style lang="scss" src="@/components/nullstyle.scss">
.app {
  background-color: #252237;
}
</style>
