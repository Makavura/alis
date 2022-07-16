<template>
  <div class="center">
    <label for="date-picker"> Please choose a date </label>
    <input
      type="date"
      id="date-picker"
      name="date-picker"
      value="2018-07-22"
      min="2018-01-01"
      max="2030-12-31"
    />
    <label for="email"> Please enter your email </label>
    <input type="email" id="email" pattern="" size="30" required />
    <input type="button" value="Send Email" />
  </div>
</template>

<script>
const todaysDate = new Date();
const todaysDateFormatted = `${todaysDate.getFullYear()}-${
  todaysDate.getMonth() + 1
}-${todaysDate.getDate()}`;

export default {
  data() {
    return {
      todaysDateFormatted,
    };
  },
};
</script>
