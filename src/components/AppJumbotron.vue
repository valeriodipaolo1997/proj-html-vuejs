<script>
export default {
    name: 'AppJumbotron',

    data() {
        return {


        }
    },

}
</script>


<template>
    <div id="jumbo">
        <div class="position-relative">
            <img class="jumbo_img" src="../assets/img/business-people-working-together-on-project-and-B3MZ4TX.jpg" alt="">
          <div class="position-absolute top-50 start-50 translate-middle text-center">
            <h1 class="text-white">LET'S TALK ABOUT WORK</h1>
            <p>A wonderful serenity has taken possession far far away, behind the word mountains</p>
            <button class="btn rounded-0"> <span>GET STARTED</span></button>
          </div>
        </div>
        
        
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

#jumbo {
    
    margin-top: 15rem;
    
   

}

.jumbo_img{
   height: 400px;
   width: 100%;
   object-fit: cover;

}

p {
  
    color: $bc_textoff-white;
    padding: 0 14rem;
    
}

.btn {
    background-color: $bc_dark;
    
    padding: 0.6rem 2.5rem;
}

span {
    font-size: 0.9rem;
    color: $bc_textoff-white;
}
</style>