<template>
  <div class="custom-check-box" @click="clickCheckBox">
    <div class="ck-box" :class="{checked:checked}"></div>
    {{ modelValue }}
  </div>
</template>

<script>
export default {
  name: 'CustomCheckBox',
  props: {
    modelValue: {
      require: true
    },
    trueValue: {
      default: ()=> {
        return true
      }
    },
    falseValue: {
      default: ()=> {
        return false
      }
    }
  },
  computed: {
    checked(){
      return this.modelValue === this.trueValue
    }
  },
  methods: {
    clickCheckBox() {
      if( this.checked ) {
        this.$emit('clickCheckBox', this.falseValue )
      } else {
        this.$emit('clickCheckBox', this.trueValue )
      }
    }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.custom-check-box {
  display: flex;

  .ck-box {
    border: 1px solid black;

    width: 30px;
    height: 30px;

    &.checked {
      background-color: black;
    }
  }

}
</style>
