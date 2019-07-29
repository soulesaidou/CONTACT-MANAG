
<template>
    <div>
        <h2>Créer un contact</h2>
        <form @submit.prevent="createContact">
            <!-- ".prevent" évite le comportement par defaut du formulaire -->
            <!-- v-on ou @ permettes (d'écouter une élément) de faire la soumission des méthode
            créer et écouté l'évenement du formulaire , dans ce cas la c'est submit -->
            <!--v-model permet de faire le lien entre le script et les template-->
            <input type ="text" placeholder = "prénom" v-model="contact.firstName"><br>
            <input type ="text" placeholder = "nom" v-model="contact.lastName"><br>
            <input type ="text" placeholder = "email" v-model="contact.email"><br>
            <input type ="text" placeholder = "téléphone" v-model="contact.phone"><br>
            <button type="submit">créer</button>
        </form>
    </div>
</template>

<script>
// import { METHODS } from 'http';
export default {
  data() {
    return {
      contact: {
        firstName: '',
        lastName: '',
        email: '',
        phone: '',
      },
    };
  },
  // methode va nous permettre de créer la soumission de notre formulaire de contact
  methods: {
    createContact() {
      console.log('this.contact');
      // pour accéder au élement du contact ont utilise l'élement this
    },
  },
};
// vdata permet de generer une structure vierge d'une fonction data
</script><style lang="scss" scoped></style>

<style scoped> /* le scoped permet de pouvoir modifier uniquement sur le composent choisie*/
h2
{
    color: red;
}
</style>
