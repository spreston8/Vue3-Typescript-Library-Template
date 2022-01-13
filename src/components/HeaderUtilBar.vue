<script>
// import { defineComponent } from 'vue';
/**
 * Provides utilities (links) above HeaderBar
 */
export default {
  name: "HeaderUtilBar",
  props: {
    /**
     * Text Color
     */
    textColor: {
      required: false,
      type: String,
    },
  },
};
</script>
<template>
  <div class="header-util-bar">
    <img class="util-bar-icon" src="" />
    About Us
    <img class="util-bar-icon" src="" />
    Locations
    <img class="util-bar-icon" src="" />
    Contact Us
  </div>
</template>
<style>
.header-util-bar {
  width: 100%;
  display: flex;
  flex: 1 1 auto;
  justify-content: flex-end;
  height: 41px;
}
.util-bar-icon {
  display: block;
  float: none;
  width: 18px;
  height: 18px;
  margin-top: 12px;
  margin-left: 22px;
}
</style>
