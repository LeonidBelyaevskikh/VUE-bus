<template>
  <div @click="emitMethod">
    CLICK ME
  </div>
</template>

<script>
import {bus} from '../bus.js';
export default {
  name: 'Component1',
  methods: {
    emitMethod () {
      bus.$emit('setNum', Math.floor(Math.random() * (10)));
    }
  }
}
</script>
