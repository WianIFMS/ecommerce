<template>
    <div>
        <form-login @user="login"></form-login>
    </div>
</template>

<script>
    import FormLogin from "../components/FormLogin";

    export default {
        name: "Login",
        components: {
            FormLogin
        },
        methods: {
            login(user) {
                this.$store.dispatch('login', user)
                    .then((response)=>{
                        console.log(response);
                        this.$router.push("/dashboard");
                    })
                    .catch((response)=>{
                        console.log(response);
                    })
            }
        }

    }
</script>

<style scoped>

</style>