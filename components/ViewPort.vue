<template>
  <section class="view-port" v-bind:class="classObject">
    <slot></slot>
  </section>  
</template>

<script>
  export default {
    data() {
      return {
        classObject: {
          row: this.row,
          position: this.position,
          alignCenter: this.alignCenter,
          justifyCenter: this.justifyCenter
        }
      } 
    },
    props: {
      position: { type: Boolean, default: false },
      row: { type: Boolean, default: false },
      alignCenter: { type: Boolean, default: false },
      justifyCenter: { type: Boolean, default: false }
    }
  }
</script>

<style>
.view-port {
  height: 100vh;
  display: flex;
}
.row {
  flex-direction: row;
}
.position {
  position: relative;
}
.alignCenter {
  align-items: center;
}
.justifyCenter {
  justify-content: center;
}
</style>
