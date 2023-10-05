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

                    <div class="line d-flex position-absolute top-50 end-0 translate-middle-y gap-2">
                        <i class="fa-sharp fa-regular fa-window-minimize"></i>
                        <p class=" text-uppercase">always the best way you need it</p>
                    </div>
                    <div>
                        <h1 class="text-white position-absolute top-50 start-100 translate-middle"> THE BEST BUSINESS CONSULTING</h1>
                    </div>

                    <div class=" d-flex position-absolute bottom-0 start-50 translate-middle-x">
                        <button class="btn rounded-0 "> <span>READ MORE</span></button>
                        <i class="fa-regular fa-circle-play ps-3 pt-2"></i>
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

      .fa-sharp {
        font-size: 2.3rem;
        color: $bc_success;
        margin-top: -1.2rem;
        padding-right: 1.5rem;
      }

      h1 {
        padding-right: 14rem;
        font-size: 5.4rem;
        line-height: 5rem;
      }
     

    .line {
       padding-bottom: 17rem;
       padding-right: 2rem;
    }

    .btn {
        margin-left: 5rem;
        margin-bottom: 15rem;
        padding: 0.6rem 2rem;
        background-color: $bc_success;
        
    }
    .btn:hover {
        background-color: $bc_warning;
        span {
            color: white;
        }
        
    }
    
    .fa-circle-play {
        color: white;
        font-size: 3rem;
        
    }
    

    p {
        color: $bc_textlight;
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

span {
    font-size: 0.9rem;
    color: $bc_textdark;
}


</style>