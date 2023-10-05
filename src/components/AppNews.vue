<script>
export default {
    name: 'AppNews',

    data() {
        return {


        }
    },

}
</script>

<template>
    <div class="container">
        <h6>BLOG</h6>
        <div class="d-flex justify-content-between pb-5">
            <h1>THE RECENT NEWS YOU MUST READ IT</h1>
            <button class="btn rounded-0"><span>VIEW ALL</span></button>
        </div>

        <div class="row">
            <div class="col-6">
                <div class="position-relative">
                    <img class="img-fluid"
                        src="../assets/img/startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg" alt="">
                    <div class="my_card position-absolute bottom-0 end-0">
                        <div>
                            <p class="my_text  pt-5">july 4,2019 by paul</p>
                            <h4 class="pb-3">Canadian Consulting Firm aquired by UK Giant</h4>

                            <p>When, while lovely valley teems whit vapour<br> around meand eridian sun strikes the
                                upper<br> impenetrable
                                foliage of my trees, and but a</p>
                        </div>
                    </div>


                </div>
            </div>
            <div class="col-6">
                <div class="position-relative">
                    <img class="img-fluid"
                        src="../assets/img/business-people-working-together-on-project-and-5FHSKBL-1390.jpg" alt="">
                    <div class="my_card position-absolute bottom-0 end-0">
                        <div>
                            <p class=" my_text pt-5">july 4,2019 by paul</p>
                            <h4 class="pb-3">Canadian Consulting Firm aquired by UK Giant</h4>

                            <p>When, while lovely valley teems whit vapour<br> around meand eridian sun strikes the
                                upper<br> impenetrable
                                foliage of my trees, and but a</p>
                        </div>
                    </div>


                </div>
            </div>
        </div>


    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.my_card {
    background-color: white;
    margin-left: 8rem;
    margin-bottom: -4rem;
    padding-left: 4rem;
    padding-right: 5rem;

}

.btn {

    padding: 0.4rem 3rem;
    background-color: $bc_success;
}

p {
    font-size: 0.9rem;
    color: $bc_textlight;
}

span {
    font-size: 0.8rem;
}

h4 {
    color: $bc_dark;
}

.my_text {
    color: $bc_warning;
}
</style>

