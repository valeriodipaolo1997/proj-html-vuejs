<script>
export default {
    name: 'AppConsulting',

    data() {
        return {


        }
    }
}

</script>

<template>
    <div class="container">
        <div class="d-flex">
            <h3 class="title col-6"> OUR CONSULTANTS CAN HELP YOU</h3>

            <div class="col-6">
                <hr>
            </div>
            
        </div>
        
        <div class="row">
            <div class="col-6">
                <h4>STATISTICAL CONSULTING</h4>
                <p>When, while lovely valley teems whit vapour<br> around meand eridian sun strikes the upper<br> impenetrable
                    foliage of my trees, and but a</p>

            </div>
            <div class="col-6">
                <h4>DIGITAL CONSULTING</h4>
                <p>When, while lovely valley teems whit vapour<br> around meand eridian sun strikes the upper<br> impenetrable
                    foliage of my trees, and but a</p>


            </div>
        </div>

        <div class="row">
            <div class="col-6">
                
                <h4>BANKING CONSULTING</h4>
                <p>When, while lovely valley teems whit vapour<br> around meand eridian sun strikes the upper<br> impenetrable
                    foliage of my trees, and but a</p>


            </div>
            <div class="col-6">
                <h4>ENTERPRISE CONSULTING</h4>
                <p>When, while lovely valley teems whit vapour<br> around meand eridian sun strikes the upper<br> impenetrable
                    foliage of my trees, and but a</p>


            </div>
        </div>

    </div>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

.row {
    padding-bottom: 6rem;
    font-family:Arial, Helvetica, sans-serif;
}

h3 {
    padding: 6rem 0;
    color: $bc_dark;
    font-weight: bold;
    
}

h4 {
    color: $bc_dark;
    padding-bottom: 1rem;
    font-weight: bold;
}

p {
    color: $bc_textlight;
    font-size: 1.2rem;
}

hr {
    border: 2px solid $bc_successlight;
    height: 5px;
    background-color: $bc_successlight;
    margin-top: 7rem;
    width: 995px;
    margin-left: -8rem;
}

</style>