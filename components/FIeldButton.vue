<template>
  <div>
    <slot name="header" />
    <br />
    <el-button> {{ txt }} <slot name="content" /> </el-button>
    <br />
    <slot name="footer" />
  </div>
</template>

<script setup>
const props = defineProps({
  txt: String,
  size: String,
  type: String,
  disabled: Boolean,
  plain: Boolean,
  round: Boolean,
  circle: Boolean,
  loading: Boolean,
});
</script>
