<template>
  <div class="affiche">
    <h1>Besoin d'inspiration ?</h1>
    <p>
      Nos ambasssadeurs sont fiers d'utiliser nos produits. Decouvrez les en
      video.
    </p>

    <br />
    <br />

    <div class="best">
      <div class="card" v-for="item in items" :key="item.id">
        <div class="overlay">
            <h2 class="text-xl" style="margin-top: 100%;">{{item.nom}}</h2>
        </div>
        <div class="img-box shadow-sm">
          <img :src="item.url" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          nom: "Claudia",
          url: "https://cdn-hosting-yam.s3.eu-west-1.amazonaws.com/wp-content/uploads/2024/01/30011201/cropped-Farine-de-patate-douce-Claudia-Modica.png",
        },

        {
          nom: "Jerome",
          url: "https://cdn-hosting-yam.s3.eu-west-1.amazonaws.com/wp-content/uploads/2024/01/30011059/cropped-Jerome-et-Enfants-font-gaufres-FARINE.png",
        },

        {
          nom: "Yohan",
          url: "https://cdn-hosting-yam.s3.eu-west-1.amazonaws.com/wp-content/uploads/2024/01/30010810/cropped-Supermag-Yohan-Taboucherani-.png",
        },

      
      ],
    };
  },
};
</script>

<style scoped>
.affiche {
  background-color: #2E2E2E;
  color: white;
  padding: 60px 20px 60px 20px;
}

.best {
  display: flex;
  align-items: start;
  width: 100%;
  height: auto;
  overflow: auto;
  padding: 10px 10px 10px 0px;
}

.card {
  min-width: 160px;
  height: auto;
  border-radius: 15px;
  margin-right: 20px;
  position: relative
}

img {
  width: 550px;
  height: auto;
  max-width: 100%;
  border-radius: 15px;
}

.img-box {
  height: auto;
  border-radius: 7px;
}
.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 10px;
  background-color: rgba(0, 0, 0, 0.325);
  border-radius: 15px;
  z-index: 1;
}

h1 {
  font-family: Montserrat;
  font-size: 1.7rem;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  color: var(--black-dark);
}
</style>