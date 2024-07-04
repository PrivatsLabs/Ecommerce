<template>
  <div class="menu-list">
    <div class="top">
      <svg
       @click="retour"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        class="size-6"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M15.75 19.5 8.25 12l7.5-7.5"
        />
      </svg>

      <p class="text-lg"><strong>Nos produits de A a Z</strong></p>

      <svg
       @click="close"
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        class="size-6"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M6 18 18 6M6 6l12 12"
        />
      </svg>
    </div>

    <br />
    <br />
    <div class="center">
      <h1><strong>A</strong></h1>

      <a href="#">Alpha X</a> <br />
      <a href="#">Anti stress</a> <br />
      <a href="#">Aphodisia</a> <br />

      <br />

      <h1><strong>A</strong></h1>

      <a href="#">Alpha X</a> <br />
      <a href="#">Anti stress</a> <br />
      <a href="#">Aphodisia</a> <br />
      <br />

      <h1><strong>A</strong></h1>

      <a href="#">Alpha X</a> <br />
      <a href="#">Anti stress</a> <br />
      <a href="#">Aphodisia</a> <br />

      <br />

      <h1><strong>A</strong></h1>

      <a href="#">Alpha X</a> <br />
      <a href="#">Anti stress</a> <br />
      <a href="#">Aphodisia</a> <br />

      <br />

      <h1><strong>A</strong></h1>

      <a href="#">Alpha X</a> <br />
      <a href="#">Anti stress</a> <br />
      <a href="#">Aphodisia</a> <br />

      <br />

      <h1><strong>A</strong></h1>

      <a href="#">Alpha X</a> <br />
      <a href="#">Anti stress</a> <br />
      <a href="#">Aphodisia</a> <br />
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return{

        }
        
    },
    methods:{
        retour(){
            document.querySelector('.menu-list').style.display='none';
        },
        close(){
            document.querySelector('.menu-list').style.display='none';
            document.querySelector('.menu').style.display='none';
        }
    }

}
</script>

<style scoped>
.menu-list {
    display: none;
  position: fixed;
  z-index: 40;
  height: 100vh;
  width: 100%;
  left: 0;
  background-color: #fff;
  padding: 20px;
  overflow: scroll;
}
.top {
  display: flex;
  align-items: center;
  justify-content: space-between;
  position: fixed;
  top: 0;
  left: 0%;
  width: 100%;
  height: 70px;
  padding: 20px;
  background-color: #fff;
}

.center {
  margin-top: 50px;
  margin-bottom: 50px;
}

.center a {
  font-size: 0.9rem;
  text-decoration: underline !important;
}
</style>