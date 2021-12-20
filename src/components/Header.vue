<template>
    <header>
        <img src="../assets/img/dc-logo.png" alt="DC Logo">
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

</style>