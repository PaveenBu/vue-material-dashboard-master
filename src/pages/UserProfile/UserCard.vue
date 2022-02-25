<template>
  <md-card class="md-card-profile">
    <md-card-content>
      <h4 class="card-title">แบบฟอร์มการ ยืม/คืน ทรัพย์สินบริษัท</h4>
      <p class="card-description">
        กรุณาเขียนชื่อ Asset ให้เหมือนกันทั้งตอน ยืม และ คืน
      </p>
    </md-card-content>
  </md-card>
</template>
<script>
export default {
  name: "user-card",
  props: {
    cardUserImage: {
      type: String,
      default: require("@/assets/img/faces/marc.jpg"),
    },
  },
  data() {
    return {};
  },
};
</script>
<style></style>
