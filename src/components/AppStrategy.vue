<script>
export default {
    name: 'AppStrategy',

    data() {
        return {


        }
    }
}

</script>

<template>
    <div class="d-flex">
        <div>
            <img height="800" src="../assets/img/business-people-working-together-on-project-and-5FHSKBL.jpg">

        </div>


        <div class="about_us container d-flex flex-column">
            <div class="d-flex">
                <hr>
                <p class="about">ABOUT US</p>
            </div>

            <h1 class="pb-4">WE MAKE YOUR STRATEGY WORK</h1>
            <p>When, while lovely valley teems whit vapour around meand eridian sun strikes the upper impenetrable
                foliage of my trees, and but a When, while lovely valley teems whit vapour around meand eridian sun
                strikes the upper impenetrable
                foliage of my trees, and but a while lovely valley teems whit vapour around meand eridian sun and but a
                while while</p>

        </div>
    </div>

    <div class="get_started">
        <div class="help container">
            <div class="row">
                <div class="col">
                    <h2>WE HELP TO DELIVER <br> THE BUSINESS CASE</h2>
                </div>
                <div class="col">
                    <p>When, while lovely valley teems whit vapour around <br> meand eridian sun strikes the upper impenetrable <br>
                        foliage of my trees  while lovely valley teems whit </p>
                </div>
            </div>
        </div>
        <div class="d-flex justify-content-end">
            <button type="button" class="btn btn-lg rounded-0">GET STARTED</button>
        </div>
        
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.about_us {

    padding-left: 5rem;
    padding-right: 15rem;
    padding-top: 15rem;

}

.about {
    color: $bc_white;
}

h1 {
    font-weight: bold;
    font-size: 3.5rem;
    line-height: 3.3rem;

}

hr {

    width: 30px;
    color: $bc_success;
}


.get_started {
    width: calc(100% - 220px);
    background-color: $bc_successlight;
}

h2 {
   padding-left: 7rem; 
   color: $bc_dark;
}

.help {
    padding-top: 6rem;
    padding-bottom: 2rem;
}

p {
    color: $bc_textlight;
}

.btn {
    background-color: $bc_warning;
    color: white;
    padding: 0.7rem 2.5rem;
    font-size: 1rem;
}


</style>