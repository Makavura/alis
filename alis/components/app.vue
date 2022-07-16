<template>
  <div class="center">
    <div>
      <input
        type="date"
        id="date-picker"
        name="date-picker"
        value="2018-07-22"
        min="2018-01-01"
        max="2030-12-31"
      />
    </div>
  </div>
</template>

<script>
const todaysDate = new Date();
const todaysDateFormatted = `${todaysDate.getYear()}-${todaysDate.getMonth()}-${todaysDate.getDate()}`;
export default {
  data() {
    return {};
  },
};
</script>
