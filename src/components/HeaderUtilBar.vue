<script>
import HeaderUtilBarLink from "./HeaderUtilBarLink.vue";
// import { defineComponent } from 'vue';
/**
 * Provides utilities (links) above HeaderBar
 */
export default {
  name: "HeaderUtilBar",
  components: { HeaderUtilBarLink },
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
    <img
      class="util-bar-icon"
      src="https://www.cnb.com/content/dam/cnb/global-assets/images/icons/topnav_contactus.svg"
    />
    <header-util-bar-link
      :textColor="textColor"
      href="https://www.cnb.com/about-us/company-overview.html"
      class="header-util-bar_icons-aboutus"
      title="About Us"
    >
      About Us
    </header-util-bar-link>
    <img
      class="util-bar-icon"
      src="https://www.cnb.com/content/dam/cnb/global-assets/images/icons/topnav_locations.svg"
    />
    <header-util-bar-link
      :textColor="textColor"
      href="https://locations.cnb.com/"
      class="header-util-bar_icons-locations"
      title="Locations"
    >
      Locations
    </header-util-bar-link>
    <img
      class="util-bar-icon"
      src="https://www.cnb.com/content/dam/cnb/global-assets/images/icons/topnav_aboutus.svg"
    />
    <header-util-bar-link
      :textColor="textColor"
      href="https://www.cnb.com/about-us/contact-us.html"
      class="header-util-bar_icons-contactus"
      title="Contact Us"
    >
      Contact Us
    </header-util-bar-link>
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
