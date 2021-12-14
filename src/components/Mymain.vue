<template>
    <div class="main-container">
        <stickyHeader :headerElements="this.headerData"/>
        <div class="site-content">
            <Myhero id="home"/>
            
        </div>    
    </div>
</template>

<script>
import Myhero from './Myhero.vue'
import stickyHeader from './stickyHeader.vue'

export default {
    name: "Mymain",
    components:{
        Myhero,
        stickyHeader,
    },
    data(){
        return{
            headerData : [
                {
                    name: 'HOME',
                    id: 'scrollHome',
                    class: 'link'
                },
                {
                    name: 'ABOUT',
                    id: 'scrollAbout',
                    class: 'link'
                },
                {
                    name: 'SERVICES',
                    id: 'scrollServices',
                    class: 'link'
                },
                {
                    name: 'PRICING',
                    id: 'scrollPricing',
                    class: 'link'
                },
                {
                    name: 'BLOG',
                    id: 'scrollBlog',
                    class: 'link'
                },
                {
                    name: 'GET IN TOUCH',
                    id: 'scrollTouch',
                    class: 'btn'
                }
            ],           
        }
    }
};
</script>

<style lang="scss">
.main-container{
    color: #e3e7df;
    position: relative;
    .site-content{
        position: relative;
        top: -82px;
    }        
}
</style>