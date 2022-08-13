<template>
    <div>

    <h1 v-for="(username,index) in usernames" :key="index" @click="highlight_username">{{username}}</h1>

    </div>
</template>

<script>
    export default {
        methods: {
            highlight_username(details) {
                let value_name = details[`target`][`innerText`];
                this.$root.$emit(`user_clicked`,value_name);
            }
        },
        data() {
            return {
                usernames: [`sam`,`nit`,`sat`,`nav`]
            }
        },
    }
</script>

<style scoped>

</style>