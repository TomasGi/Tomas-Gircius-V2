<template>
    <div>
        <div class="background-fixed can-toggle-menu"></div>
        <div class="main-menu-admin main-menu">
            <div class="menu-header">
                <button class="close-button can-toggle-menu">
                    <i class="material-icons">&#xE5CD;</i>
                </button>
            </div>
            <nav>
                <nuxt-link to="/" data-ref=".contact" class="item can-toggle-menu scroll-toggle">
                    Contact
                </nuxt-link>
                <nuxt-link to="/" data-ref=".canvas-holder" class="item can-toggle-menu scroll-toggle">
                    Tech
                </nuxt-link>
            </nav>
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>