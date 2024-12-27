
<template>
  <div class="popup-overlay" @click.self="close">
    <div class="popup-content">
      <button class="popup-close" @click="close">✖</button>
      <div class="popup-header">
        <slot name="header"></slot>
      </div>
      <div class="popup-body">
        <slot name="content"></slot>
      </div>
    </div>
  </div>
</template>

<script>

export default {
    methods: {
      close() {
        this.$emit("close");
      },
    },
  };

</script>

<style>

.popup-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 1000;
}

.popup-content {
  background: white;
  padding: 20px;
  border-radius: 10px;
  position: relative;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);
  max-width: 600px;
  width: 90%;
  text-align: left; /* Ensure text aligns properly for readability */
  color: black; /* Set default text color to black */
}

.popup-close {
  position: absolute;
  top: 10px;
  right: 10px;
  background: none;
  border: none;
  font-size: 1.5em;
  cursor: pointer;
  color: #555; /* Soft gray for the close button */
  transition: color 0.3s ease;
}

.popup-close:hover {
  color: #000; /* Darker color on hover for better visibility */
}

.popup-header {
  font-size: 1.8em; /* Larger font size for header */
  font-weight: bold;
  color: #000; /* Explicitly set header text color to black */
  margin-bottom: 15px;
  border-bottom: 2px solid #ddd; /* Subtle divider under the header */
  padding-bottom: 10px;
}

.popup-body {
  font-size: 1.2em; /* Slightly larger font for content readability */
  color: #000; /* Explicitly set body text color to black */
  line-height: 1.6; /* Comfortable line spacing */
}

</style>