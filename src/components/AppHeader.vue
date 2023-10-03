<script>
export default {
    name: 'AppHeader',

    data() {
        return {
            activeLink: 0,
            navItems: ['home', 'about', 'projects', 'services', 'blog', 'contact']

        }
    }
}
</script>

<template>
    <header>




        <div class="header_top d-flex">
            
                <div class="header_left position-relative">
                    <img height="20" class="logo" src="../assets/img/logotype.png" alt="logo">

                    <div class="line d-flex position-absolute top-50 end-0 translate-middle-y">
                        <hr>
                        <p class="text-white text-uppercase">always the best way you need it</p>
                    </div>
                    <div>
                        <h1 class="text-white position-absolute top-50 start-100 translate-middle"> THE BEST BUSINESS CONSULTING</h1>
                    </div>

                    <div class=" d-flex position-absolute bottom-0 start-50 translate-middle-x">
                        <button class="btn rounded-0 "> READ MORE</button>
                        <i class="ps-4 pt-2">
                            <img height="40" class="logo_play" src="../assets/img/play-button.png" alt="">
                        </i>
                    </div>
                </div>

                <div class="header_right d-flex flex-row-reverse">
                    <div class="menu">
                        <nav class="navbar navbar-expand navbar-light">
                            <ul v-for="(item, index) in navItems" class="nav navbar-nav">
                                <li class="nav-item" @click="activeLink = index">
                                    <a class="nav-link" :class="activeLink === index ? 'active' : ''" href="#"
                                        aria-current="page">{{ item }}</a>
                                </li>
                            </ul>
                        </nav>
                    </div>
                </div>
            


        </div>


    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

header {
    

    .header_top {
        li {
            a {
                text-transform: uppercase;
                color:$bc_textlight;

                &.active {
                    color: $bc_white;
                }
            }

            & a.active {
                border-top: 2px solid;

            }
        }
    }

    .header_left {
        width: 600px;
        height: 900px;
        background-color: $bc_dark;
      .logo {
        margin-top: 1rem;
        padding-left: 15rem;
      }

      hr {
    
        width: 30px;
        color: $bc_success;
      }

      h1 {
        padding-right: 14rem;
        font-size: 5rem;
        line-height: 5rem;
      }
     

    .line {
       padding-bottom: 17rem;
       padding-right: 2rem;
    }

    .btn {
        margin-left: 5rem;
        margin-bottom: 15rem;
        padding: 0.5rem 2rem;
        background-color: $bc_success;
    }

    .logo_play {
        color: $bc_success;
    }
      
    }

    .header_right {
        height: 900px;
        width: calc(100% - 600px);
        background-image: url(../assets/img/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg);
        .menu{
            padding-right: 6rem;
        }
    }


}
</style>