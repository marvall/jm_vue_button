<template>
    <button class="jm_button_style" @click="handleButtonClick">{{name}}</button>
</template>

<script>
export default {
  name: "jm_Button",
  props: ['name'],
  methods:{
      handleButtonClick($event){
          this.$emit('handleClick', $event)
      },
  }
};
</script>
<style scoped lang="scss">
    .jm_button_style {
        padding: 5px 20px;
        background-color: rgb(78, 78, 197);
        border: 1px solid rgb(50, 50, 204);
        border-radius: 25px;
        box-shadow: 1px 1px 5px rgb(46, 45, 45);
        min-width: 120px;
        font-weight: 700;
        font-size: 20px;
        color: rgb(219, 218, 255);
        text-shadow: 1px 1px 3px rgb(150, 147, 228);
    }
</style>