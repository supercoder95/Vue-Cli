<template>
  <div>
    <app-header 
    v-bind:propsdata="str"
    v-on:renew="renewStr"></app-header>
  </div>
</template>

<script>
import Appheader from './components/AppHeader';

export default {
  data: function() {
    return {
      str: 'Header'
    }
  },
  components: {
    'app-header': Appheader
  },
  methods: {
    renewStr: function() {
      this.str = 'hi';
    }
  }
}
</script>
 
<style>

</style>