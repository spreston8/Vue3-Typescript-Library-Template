<script>
// import { defineComponent } from 'vue';

export default {
  name: "HeaderUtilBarLink",
  inheritAttrs: false,
  props: {
    href: { type: String, required: true },
    textColor: { type: String, required: false, default: "#fff" },
  },
};
</script>

<template>
  <a
    v-bind="$attrs"
    :href="href"
    :style="{ color: textColor }"
    class="header-util-bar-link"
  >
    <slot></slot>
  </a>
</template>
<style>
a.header-util-bar-link {
  display: flex;
  align-items: center;
  font-size: 16px;
  text-decoration: none;
  margin-left: 10px;
}
</style>
