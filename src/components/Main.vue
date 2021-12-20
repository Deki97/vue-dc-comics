<template>
    <main>
        <div class="container">
            <div class="content">
                Content goes here
            </div>
        </div>
    </main>
</template>


<script>
export default {
    name: "Main",
    data: function() {
        return {
            
        }
    }
}
</script>


<style lang="scss" scoped>
main {
    background-color: #1c1c1c;

    .content {
        color: white;
        font-size: 24px;
        padding: 40px 0;

        &::before {
            content: '-->';
        }

        &::after {
            content: '<--';
        }
    }
}
</style>