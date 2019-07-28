<template>
    <div>
        <form action="">
            <input type ="text"> placeholder = "prénom">
            <input type ="text"> placeholder = "nom">
            <input type ="text"> placeholder = "email">
            <input type ="text"> placeholder = "téléphone">
            <button type="submit">créer</button>
        </form>
    </div>
</template>

<script>
    export default {
        data(){
            return{
              firstName: "",
              lastName: "",
              email: "",
              phone: ""
            };
        }
    }
</script>

<style lang="scss" scoped>

</style>
