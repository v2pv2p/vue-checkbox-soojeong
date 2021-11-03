<template>
  <div class="main">
    <div>메인</div>
    <custom-check-box :modelValue="checkBoxData"
                      :falseValue="false"
                      :trueValue="true"
                      @clickCheckBox="checkBoxData = $event"
    ></custom-check-box>
  </div>
</template>

<script>
import CustomCheckBox from '@/components/CustomCheckBox'

export default {
  name: 'Main',
  components: { CustomCheckBox },
  component: {
    CustomCheckBox
  },
  data() {
    return {
      checkBoxData: '',
    }
  },
  methods: {}
}
</script>

<style scoped>

</style>
