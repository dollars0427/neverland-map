<template>
  <div ref="pointer" class="pointer" />
</template>

<script>
export default {
  name: 'pointer',
  props: {
    position: Object,
  },
  created(){
    const canvas = this.$refs.pointer;
    if (canvas.getContext){
      const ctx = canvas.getContext('2d');
      ctx.beginPath();
      ctx.arc(75,75,50,0, Math.PI*2,true); // Outer circle
      ctx.stroke();
    }
  },
}
</script>
