<template>
  <div class="map">
    <img src="../assets/map.jpg" class="img-responsive" />
    <pointer></pointer>
  </div>
</template>

<script>
import pointer from './pointer';
export default {
  name: 'map',
  components: {
    pointer,
  }
}
</script>
