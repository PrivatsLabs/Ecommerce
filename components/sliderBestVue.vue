<template>
  <div class="best">
    <div class="card" v-for="item in items" :key="item.id">
      <div class="img-box shadow-sm">
        <img
          :src="item.url"
          
        />
      </div>
      <div class="info-box">
        <p class="h2">{{item.nom}}</p>
        <p class="subtit">{{item.info}}</p>

        <span>{{item.prix}}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return{
      items:[
        {nom: 'Farine de patate douce', info: 'Notre produit phare',prix: '19.99 £', url: 'https://cdn-hosting-yam.s3.eu-west-1.amazonaws.com/wp-content/uploads/2021/01/03154029/ikk.webp'},

        {nom: 'deuxieme', info: 'info',prix: '19 £', url: 'https://cdn-hosting-yam.s3.eu-west-1.amazonaws.com/wp-content/uploads/2024/01/29113115/Virilis-120-comprimes.png'},

        {nom: 'nom', info: 'info',prix: '19 £', url: 'https://cdn-hosting-yam.s3.eu-west-1.amazonaws.com/wp-content/uploads/2024/01/29191911/mock-up-optivegan-cacao-1.png'},

        {nom: 'nom', info: 'info',prix: '19 £', url: 'url'},
        {nom: 'nom', info: 'info',prix: '19 £', url: 'url'},
      ]
    }
  },
}
</script>

<style scoped>

.best {
  display: flex;
  align-items: start;
  width: 100%;
  height: auto;
  overflow: auto;
  padding: 10px 10px 10px 0px;
}

.card{
    min-width: 220px;
    height: auto;
    border-radius: 15px;
    margin-right: 20px;
}

img {
  width: 550px;
  height: auto;
  max-width: 100%;

}

.img-box {
    background-color: #F5F4F0;
    height: 240px;
    border-radius: 7px;

}

.info-box{
    padding: 10px 10px 10px 0px;
    height: auto;

}

.h2 {
  font-family: Montserrat;
  font-size: 18px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  color: var(--black-dark);
}
.subtitle {
  font-size: 15px;
}
.info-box span{
    font-weight: bolder;
}
</style>

