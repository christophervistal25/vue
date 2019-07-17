<template>
    <div>
        <h1>Users View</h1>
        <button @click="proceedToHome">Click to back home!</button>
    </div>
</template>
<script>
 export default  {
     watch : {
        '$route' (to, from) {
            // alert(to.params.teamId);
        }
     },
     created() {
        // alert(this.$route.params.teamId);
     },
     methods : {
        proceedToHome() {
            this.$router.push('/');
        }
     }
}
</script>