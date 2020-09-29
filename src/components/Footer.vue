<template>
  <div class = "footer">
    <div class = "footer-box">
      <slot ></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
 .footer {
   position: relative;
   height: 100px;
   width: 100%;
 }


 .footer-box {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 0 100px;
    height: 100%;
 }
</style>
