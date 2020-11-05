<template>
  <div>
    {{num}}
  </div>
</template>

<script>
import {bus} from '../bus.js';

export default {
  name: 'Component3',
  data: function () {
    return {
      num: 0
    }
  },
  mounted() {
    bus.$on('setNum', data => {
      this.num = data
    })
  }
}
</script>
