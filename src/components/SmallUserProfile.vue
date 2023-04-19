<template>
  <div>
  <h3>{{user[`name`]}}</h3>
  <p>{{user[`age`]}}</p>
  <h4 v-if="user[`is_premium`]===true">premium</h4>
  <p v-else>Basic</p>
  </div>
</template>

<script>
export default {
props: {
    user: Object,
}
};
</script>

<style scoped>
/* add your styles here */
</style>
