<script>
export default {
    name: 'AppHelp',

    data() {
        return {


        }
    },

}

</script>

<template>
    <div class="help_clients container">
        <div class="d-flex">
                <i class="fa-sharp fa-regular fa-window-minimize"></i>
                <p class="project">PROJECT</p>
            </div>
        <div class="d-flex justify-content-between">
            <h1 class="pb-4 text-white">OUR EXPERT TRUSTED CONSULTANTS <br> HELP CLIENTS</h1>
            <div class="pt-2">
                <button class="btn btn-primary rounded-0 me-2"><i class="fa-solid fa-arrow-right-long"></i></button>
                <button class="btn btn-primary rounded-0"><i class="fa-solid fa-arrow-right-long fa-rotate-180"></i></button>
            </div>

        </div>

        <div class="row">
            <div class="col">
                <img src="../assets/img/DRY-1-790x592.jpg" alt="">
            </div>
            <div class="col">
                <img src="../assets/img/221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg" alt="">
            </div>
            <div class="col">
                <img src="../assets/img/z1el4c4p-790x592.jpg" alt="">
            </div>
        </div>

        <h6 class="d-flex justify-content-center">TESTIMONIAL</h6>
        <i class="fa-sharp fa-regular fa-window-minimize d-flex justify-content-end text-end p-0"></i>
        <h1 class="d-flex justify-content-end text-end pb-5 text-white">WHAT'S THE CUSTOMERS SAY <br> ABOUT YOUR WORK</h1>


        <div class="my_container container">
            <div class="row p-4">
                <div class="col px-5">
                    <p>
                        When, while lovely valley teems whit vapour around meand eridian sun strikes the upper impenetrable
                        foliage of my trees, and but a When, while lovely valley teems whit vapor around meand eridian sun
                        strikes. 
                    </p>
                  <h4 class="pt-4">Vera Duncan</h4>
                  <p>Amazon Inc.</p>
                </div>
                <div class="col px-5">
                    <p>
                        When, while lovely valley teems whit vapour around meand eridian sun strikes the upper impenetrable
                        foliage of my trees, and but a When, while lovely valley teems whit vapor around meand eridian sun
                        strikes.
                    </p>
                    <h4 class="pt-4">Vera Duncan</h4>
                    <p>Amazon Inc.</p>
                </div>
                <div class="col px-5">
                    <p>
                        When, while lovely valley teems whit vapour around meand eridian sun strikes the upper impenetrable
                        foliage of my trees, and but a When, while lovely valley teems whit vapor around meand eridian sun
                        strikes. 
                    </p>
                    <h4 class="pt-4">Vera Duncan</h4>
                    <p>Amazon Inc.</p>
                </div>
            </div>
        </div>

    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.my_container {
    background-color: white;
    
}
img {

max-width: 100%;
}

.help_clients {
    padding: 8rem 0;
}

h6 {
    padding-top: 6rem;
    color: $bc_textlight;
}

p {
    font-size: 0.9rem;
    color: $bc_textlight;
}

.fa-sharp {
        font-size: 2.3rem;
        color: $bc_success;
        margin-top: -1.2rem;
        padding-right: 1.5rem;
      }

.project {
    color: $bc_textoff-white;
    font-size: 1rem;
}      


.btn {
    background-color: $bc_gray;
    border: none;

}


h4 {
    color: $bc_dark;
}

</style>