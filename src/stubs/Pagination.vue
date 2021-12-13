<template>
  <div :style="{ display: 'flex', justifyContent: 'center', width: '100%'}">
    <a-pagination v-model="current" :total="50" show-less-items />
  </div>
</template>
<script>
export default {
  data() {
    return {
      current: 2,
    };
  },
};
</script>
