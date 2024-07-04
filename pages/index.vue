<template>
  <div class="wrapper">
    <br> <br> <br>
    <img
      src="https://cdn-hosting-yam.s3.eu-west-1.amazonaws.com/wp-content/uploads/2023/03/02155535/Banniere-mobile.png"
      alt=""
    />

    <br />
    <br />

    <div class="meilleur">
      <h1>
        Nos meilleures <br />
        ventes
      </h1>
      <br />

      <sliderBestVue></sliderBestVue>

      <br />
      <br />
    </div>

    <afficheVue></afficheVue>

    <br />
    <br />
    <div class="center">
      <h1>Nos proteines</h1>
      <br />

      <proteinesVue></proteinesVue>

      <br />
      <br />
      <br />

      <hr />

      <br />
      <br />
      <br />

      <h1>Nos vitamines</h1>
      <br />

      <vitaminesVue></vitaminesVue>

      <br />
      <br />

      <div class="apropos shadow-sm">
        <h1>Qui sommes-noux ?</h1>
        <br />

        <p>
          Présent dans le monde du fitness et du sport depuis plus de 30 ans,
          Christophe Bonnefont est non seulement un entrepreneur à succès mais
          avant tout un expert incontesté en transformations corporelles et
          dépassement de soi. Et pour cause ! Pratiquant acharné en musculation
          depuis ses 12 ans…
        </p>
        <br />

        <a href="#">En savoir plus</a>
      </div>

      <br />
      <br />

      <h1>Nos complement sportifs</h1>
      <br />

      <sportifVue></sportifVue>

      <br />
      <br />
    </div>

    <div class="confiance-icon">
      <div>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="lucide lucide-leaf"
        >
          <path
            d="M11 20A7 7 0 0 1 9.8 6.1C15.5 5 17 4.48 19 2c1 2 2 4.18 2 8 0 5.5-4.78 10-10 10Z"
          />
          <path d="M2 21c0-3 1.85-5.36 5.08-6C9.5 14.52 12 13 13 12" />
        </svg>
        <p>A base de produits <strong>naturels</strong></p>
      </div>

      <div>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="lucide lucide-shield-check"
        >
          <path
            d="M20 13c0 5-3.5 7.5-7.66 8.95a1 1 0 0 1-.67-.01C7.5 20.5 4 18 4 13V6a1 1 0 0 1 1-1c2 0 4.5-1.2 6.24-2.72a1.17 1.17 0 0 1 1.52 0C14.51 3.81 17 5 19 5a1 1 0 0 1 1 1z"
          />
          <path d="m9 12 2 2 4-4" />
        </svg>
        <p>Haut qualite <strong>nutritionnelle</strong></p>
      </div>

      <div>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="lucide lucide-map-pin"
        >
          <path d="M20 10c0 6-8 12-8 12s-8-6-8-12a8 8 0 0 1 16 0Z" />
          <circle cx="12" cy="10" r="3" />
        </svg>
        <p>produit local <strong>France</strong></p>
      </div>

      <div>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="lucide lucide-car"
        >
          <path
            d="M19 17h2c.6 0 1-.4 1-1v-3c0-.9-.7-1.7-1.5-1.9C18.7 10.6 16 10 16 10s-1.3-1.4-2.2-2.3c-.5-.4-1.1-.7-1.8-.7H5c-.6 0-1.1.4-1.4.9l-1.4 2.9A3.7 3.7 0 0 0 2 12v4c0 .6.4 1 1 1h2"
          />
          <circle cx="7" cy="17" r="2" />
          <path d="M9 17h6" />
          <circle cx="17" cy="17" r="2" />
        </svg>
        <p>Livraison<strong> 24h</strong></p>
      </div>
    </div>

    <br />
    <br />

    <h1 style="margin-left: 15px">Notre gamme bien-etre</h1>
    <br />

    <bien-etreVue></bien-etreVue>

    <br />
    <br />
    <br />

    <br> <br> <br>

    <hr>

    <br> <br> <br>


  </div>
</template>
<style scoped>
h1 {
  font-size: 30px !important;
  font-style: normal !important;
  font-weight: 700 !important;
  line-height: normal;
}

.meilleur {
  padding: 15px;
}

.center {
  padding: 15px;
}

.apropos {
  padding: 15px;
  color: white;
  background-color: #2e2e2e;
  border-radius: 10px;
}
.apropos p {
  color: rgb(213, 207, 207);
}

.confiance-icon {
  background-color: #2e2e2e;
  color: white;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.confiance-icon div {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 50px;
}
.confiance-icon svg {
  width: 65px;
  height: 65px;
}

.card {
  width: 90%;
  height: 254px;
  padding: 0 15px;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 12px;
  background: #fff;
  border-radius: 20px;
  border: 1px solid grey;
  margin: 15px;
}

.card > * {
  margin: 0;
}

.card__title {
  font-size: 23px;
  font-weight: 900;
  color: #333;
}

.card__content {
  font-size: 13px;
  line-height: 18px;
  color: #333;
}

.card__form {
  display: flex;
  flex-direction: column;
  gap: 10px;
  width: 100%;
}

.card__form input {
  margin-top: 10px;
  outline: 0;
  background: rgb(255, 255, 255);
  box-shadow: transparent 0px 0px 0px 1px inset;
  padding: 0.6em;
  border-radius: 14px;
  border: 1px solid #333;
  color: black;
}

.card__form button {
  border: 0;
  background: #111;
  color: #fff;
  padding: 0.68em;
  border-radius: 14px;
  font-weight: bold;
}

.sign-up:hover {
  opacity: 0.8;
}
</style>