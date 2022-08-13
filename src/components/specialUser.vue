<template>
  <div>
    <div>
        <h1>{{dis_user}}</h1>
    </div>
  </div>
</template>

<script>
export default {
 
  methods: {
    display(value_name) {
      this.dis_user = value_name;
    }
  },
 mounted(){
    this.$root.$on(`user_clicked`,this.display);
  },
    data() {
    return {
      dis_user: undefined
    }
  },
};
</script>

<style scoped></style>
