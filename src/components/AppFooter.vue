<script>
export default {
    name: 'AppFooter',

    data() {
        return {

            activeFooter: 0,
            navFooter: ['home', 'about', 'projects', 'services', 'blog', 'contact']

        }
    },

}
</script>


<template>
    <footer>
        <div class="container d-flex justify-content-md-between pt-5 ">
            <div class="my_logo pt-2">
                <img height="20" src="../assets/img/logotype-2-150x25.png" alt="">
            </div>

            <div class="menu">
                <nav class="navbar navbar-expand navbar-light">
                    <ul v-for="(item, index) in navFooter" class="nav navbar-nav">
                        <li class="nav-item" @click="activeFooter = index">
                            <a class="nav-link" :class="activeFooter === index ? 'active' : ''" href="#"
                                aria-current="step">{{ item }}</a>
                        </li>
                    </ul>
                </nav>
            </div>

            <div class="my_icon pt-2">

                <i class="fa-brands fa-instagram"></i>
                <i class="fa-solid fa-info"></i>
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
            </div>



        </div>
        <div class="container pt-5 pb-2 px-0">
            <hr>
        </div>

        <div class="footer_bottom container d-flex justify-content-between">
            <div class="d-flex flex-column">
                <a href="#">Terms of use</a>
                <a href="#">Privacy Environmental Policy</a>
            </div>

            <div class="d-flex">
                <div>
                    <a href="#">Copyright @ 2020 Phlox Consulting.All Rights Reserved.</a>
                </div>

                <div class="icon_bottom d-flex">
                    <i class="fa-solid fa-circle-up"></i>

                    <i class="fa-solid fa-circle"></i>

                </div>

            </div>
        
        </div>
    </footer>
</template>
    
    

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;


footer {
    background-color: $bc_dark;


}

.menu {
    text-transform: uppercase;
    font-size: 0.9rem;
}

i {
    color: white;
    padding: 0 0.5rem;
}

li {
    a {

        color: $bc_textlight;

        &.active {
            color: white;
        }
    }


}

hr {
    width: 100%;
    color: $bc_textlight;

}

.footer_bottom {
    padding: 2rem 0;

    a {
        text-decoration: none;
        color: $bc_textlight;
    }
}

.icon_bottom {
    margin-right: -7rem;

    .fa-circle {
        padding-bottom: 2rem;
        font-size: 3rem;
        color: $bc_blu;
        margin-top: -1.2rem;

    }

    .fa-circle-up {
        font-size: 1.8rem;
        margin-top: -1rem;
    }


}
</style> 