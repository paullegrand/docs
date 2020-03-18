<template>
  <component
    class="browser-shot"
    :is="link? 'a' : 'div'"
    :href="link ? url : ''"
    target="_blank"
    rel="noopener"
  >
    <div class="browser-top"></div>
    <div class="address-bar">
      <div class="address">{{ getDisplayUrl(url) }}</div>
    </div>
    <div class="image">
      <slot></slot>
    </div>
  </component>
</template>

<style>
.browser-shot {
  display: block;
  position: relative;
  margin-top: 2em;
  margin-bottom: 2em;
  box-shadow: 0 0 48px rgba(74, 124, 246, 0.1);
  background: transparent;
  border-radius: 6px;
}

.browser-top {
  border-top-right-radius: 6px;
  border-top-left-radius: 6px;
  height: 22px;
  background: #e5edfd url("../../images/window-buttons.svg") no-repeat left
    center;
  background-size: auto 18px;
}

.address-bar {
  display: block;
  background-color: #e5edfd;
  padding: 0 0.5em 0.5em 0.5em;
}

.address {
  color: #2c3e50;
  background: rgba(255, 255, 255, 0.5);
  font-weight: normal;
  display: block;
  padding: 0.125em 0.25em;
  font-size: 0.75em;
  text-decoration: none;
}

.browser-shot:hover {
  text-decoration: none !important;
}

.browser-shot .image {
  position: relative;
  border-bottom-right-radius: 6px;
  border-bottom-left-radius: 6px;
  overflow: hidden;
  background-color: transparent;
}

.browser-shot .image img {
  position: relative;
  display: block;
}
</style>

<script>
export default {
  props: {
    url: {
      type: String,
      required: true
    },
    link: {
      type: Boolean,
      required: false
    },
    cleanUrl: {
      type: Boolean,
      require: false,
      default: true
    }
  },
  methods: {
    getDisplayUrl(url) {
      if (!this.cleanUrl) {
        return url;
      }

      // remove protocol and trailing slash
      return url
        .replace("https://", "")
        .replace("http://", "")
        .replace(/\/$/, "");
    }
  }
};
</script>