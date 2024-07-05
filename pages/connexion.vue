<template>
  <div class="wrapper">
    <br />
    <br />
    <br />

    <div class="connexion" v-if="etat=='co'">
      <h1 class="text-lg"><strong>Connexion</strong></h1>
      <br />
      <span>Bon retour parmi nous !</span> <br />
      <br />

      <form id="form">
        <label for="email">E-mail</label> <br />
        <input type="text" name="email" id="email" required /> <br />
        <br />

        <label for="password">Mot de passe</label><br />
        <input type="password" name="password" required /> <br />
        <br />

        <a @click="creer">Creer un compte ?</a> <br />
        <br />

        <button type="submit">Se connecter</button>
      </form>
    </div>

    <div class="inscription" v-else>
     
      <h1 class="text-lg"><strong>Inscription</strong></h1>
      <br />
      <span>Bienvenue dans la famille ❤️</span> <br />
      <br />

      <form id="form">
        <label for="prenom">Prenom</label> <br />
        <input type="text" name="id" id="prenom" required /> <br />
        <br />

        <label for="nom">Nom</label><br />
        <input type="text" name="nom" id="nom" required /> <br />
        <br />

        <label for="id">E-mail</label> <br />
        <input type="email" name="id" id="email" required /> <br />
        <br />

        <label for="password">Mot de passe</label><br />
        <input type="password" name="password" required /> <br />
        <br />

        <a @click="co">Se connecter ?</a> <br />
        <br />

        <button type="submit">Creer un compte</button>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      etat: "co",
    };
  },
  methods:{
    creer(){
        this.etat= 'ins'
  },
    co(){
        this.etat= 'co'
  },
  }
};
</script>


<style scoped>
.wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 20px;
  margin-bottom: 200px;
}

.inscription, .connexion{
    width: 100%;
}

form {
  width: 100%;
}

h1,
p, span {
  text-align: center;
}

.wrapper input {
  width: 100%;
  height: 45px;
  border: 1px solid rgba(128, 128, 128, 0.314);
  border-radius: 7px;
  padding-left: 10px;
}
input:focus {
  outline: none;
}

button {
  display: flex;
  padding: 12px 22px;
  justify-content: center;
  align-items: center;
  gap: 8px;
  border-radius: 4px;
  background: var(--black, #2e2e2e);
  color: #fff;
  font-family: Montserrat;
  font-size: 15px;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
  text-decoration: none;
  width: 100%;
}

a {
  font-size: 0.8rem;
  text-decoration: underline;
}
</style>