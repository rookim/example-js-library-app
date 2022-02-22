<script>
import flatpickr from "flatpickr";
export default {
  data: function () {
    return {
      message: "Testing out flatpickr!",
    };
  },
  created: function () {},
  methods: {},
  components: {},
};
var config = {
  enableTime: true,
  dateFormat: "Y-m-d H:i",
  altInput: true,
  altFormat: "F j, Y (h:S K)",
  minDate: "2020-01",
};
flatpickr("input[type=datetime-local]", config);
</script>

<template>
  <div class="home">
    <h1>{{ message }}</h1>
    <input type="datetime-local" placeholder="Select date and time" />
  </div>
</template>

<style></style>
