<template>
    <span class="itemStyle">{{ item.message }}</span>
</template>

<script>
export default {
  props: {
    item: Object,
  },
};
</script>

<style>
.itemStyle {
  text-decoration: line-through;
}
</style>
