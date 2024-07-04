<template>
  <div class="menu" id="menu">
    <div class="menu-top">
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

    <div class="AZ shadow-sm">
      <span class="text-sm"> <strong> Nos produits de A a Z</strong></span>

      <svg
        @click="az"
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
          d="M17.25 8.25 21 12m0 0-3.75 3.75M21 12H3"
        />
      </svg>
    </div>

    <div class="items">

        <div>
            <p>Farine de patate douce</p>
        </div>
        <div>
            <p>Proteine</p>
        </div>
        <div>
            <p>Complement sportifs</p>
        </div>
        <div>
            <p>Vitamines & bien-etre</p>
        </div>

    </div>

    <br>

    <div class="AZ shadow-sm">
      <span class="text-sm"> <strong> Nos conseils</strong></span>

      <svg
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
          d="M17.25 8.25 21 12m0 0-3.75 3.75M21 12H3"
        />
      </svg>
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
        az(){
            document.querySelector('.menu-list').style.display='block';
        },
        close(){
            document.querySelector('.menu').style.display='none';
        }
    }

}
</script>



<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100..900;1,100..900&display=swap");

* {
  margin: 0%;
  padding: 0%;
  box-sizing: border-box;
  font-family: "Montserrat";
}

.menu {
  display: none;
  padding: 20px;
  position: fixed;
  z-index: 30;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #fff;
}
.menu-top {
  width: 100%;
  height: 40px;
  display: flex;
  margin-bottom: 25px;
}

.menu-top svg {
  margin-left: auto;
  width: 30px;
  height: 38px;
}

.AZ {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  padding: 10px;
  height: 55px;
  border-radius: 10px;
  background-color: #f5f4f0;
}

.items{

    border: 1px solid #cac9c5;
    border-radius: 7px;
    padding: 10px;
    margin-top: 20px;

}

.items div{
    background-color: #f5f4f0;
    padding: 10px;
    margin: 15px;
    height: 50px;
    border-radius: 7px;
    display: flex;
    align-items: center;
}
.items p{
    font-size: 1rem;
    color: rgba(0, 0, 0, 0.674);
}
</style>