<template>
  <div class="custom-check-box" :class="{checked:checked}">

  </div>
</template>

<script>
export default {
  name: 'CustomCheckBox',
  data(){
    return {
      checked: false
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.custom-check-box {
  .checked {

  }
}
</style>
