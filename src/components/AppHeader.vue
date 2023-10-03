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
        <div class="container">
            <div class="header_top d-flex justify-content-between align-items-center">
                <div class="logo">
                    <img class="logo_img" src="../assets/img/logotype.png" alt="logo">
                </div>

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
header {
    .header_top {
        li {
        a {
            text-transform: uppercase;

            &.active {
                color: antiquewhite;
            }
        }
        & a.active {
            border-top: 2px solid;
        }
    }
    }
    
}
</style>