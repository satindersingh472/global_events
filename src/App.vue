<template>
  <div id="app">
    <user-list></user-list>
    <special-user> </special-user>
  </div>
</template>

<script>
import UserList from "@/components/userList.vue";
import SpecialUser from "@/components/specialUser.vue";

export default {
  name: "App",
  components: {
    UserList,
    SpecialUser,
  },
};
</script>

<style></style>
