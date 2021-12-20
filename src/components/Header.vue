<template>
    <header>
        <div class="container">
            <nav>
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="DC Logo">
                </div>

                <div class="menu">
                    <ul>
                        <li v-for="(menu, index) in menus" :key="index">
                            <a :href="menu.url">
                                {{ menu.text }}
                            </a>
                        </li>
                    </ul>
                </div>
            </nav>
        </div>
    </header>
</template>


<script>
export default {
    name: "Header",
    data: function() {
        return {
           menus: [
               {
                   text: 'CHARACTERS',
                   url: '#',
                   active: false
               },
               {
                   text: 'COMICS',
                   url: '#',
                   active: true
               },
               {
                   text: 'MOVIES',
                   url: '#',
                   active: false
               },
               {
                   text: 'TV',
                   url: '#',
                   active: false
               },
               {
                   text: 'GAMES',
                   url: '#',
                   active: false
               },
               {
                   text: 'COLLECTIBLES',
                   url: '#',
                   active: false
               },
               {
                   text: 'VIDEOS',
                   url: '#',
                   active: false
               },
               {
                   text: 'FANS',
                   url: '#',
                   active: false
               },
               {
                   text: 'NEWS',
                   url: '#',
                   active: false
               },
               {
                   text: 'SHOP',
                   url: '#',
                   active: false
               }
           ]
        }
    }
}
</script>


<style lang="scss" scoped>

header {
    height: 100px;
}

.container {
    nav {
        display: flex;
        justify-content: space-between;
        line-height: 100px;

        .logo {
            height: 100%;
            width: 80px;

            img {
                vertical-align: middle;
            }
        }

        .menu li {
            display: inline-block;
            font-size: 12px;
            padding: 0 10px;
        }
    }
    
}
</style>