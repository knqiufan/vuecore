<template>
    <section class="app-main">
        <transition name="fade-transform" mode="out-in">
            <keep-alive :include="cacheViews">
                <router-view :key="key"></router-view>
            </keep-alive>
        </transition>
    </section>
</template>

<script>
export default {
    name: "AppMain",
    computed:{
        cacheViews(){
            
        },
        key(){
            
        }
    }
}
</script>

<style scoped>

</style>


