<template>
  <router-view></router-view>
</template>

<script>
export default {
  name: 'App',
  created() {
    this.$store.dispatch("autoSignin");
    console.log(this.$store);
  },
}
</script>

<style>
@import "~bootstrap/dist/css/bootstrap.min.css";
@import "~@fortawesome/fontawesome-free/css/all.min.css";
@import "~animate.css/animate.min.css";
.bg-vue {
  background-color: rgb(52, 73, 94);
  color: white;
}
.bg-vue2 {
  background-color: rgb(65, 184, 131);
  color: white;
}
.text-vue {
  color: rgb(52, 73, 94)
}
.text-vue2 {
  color: rgb(65, 184, 131)
}
</style>
