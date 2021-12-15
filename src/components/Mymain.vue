<template>
    <div class="main-container">
        <stickyHeader :headerElements="this.headerData"/>
        <div class="site-content">
            <Myhero id="home"/>
            <cards />
            <aboutNetwork />
            <businessArea />
             <pricing />
             <news />
              <newsletter />
              <message />
        </div>    
    </div>
</template>

<script>
import Myhero from './Myhero.vue'
import stickyHeader from './stickyHeader.vue'
import cards from './cards.vue'
import aboutNetwork from './aboutNetwork.vue'
import businessArea from './businessArea.vue'
import pricing from './pricing.vue'
import news from './news.vue'
import newsletter from './newsletter.vue'
import message from './message.vue'

export default {
    name: "Mymain",
    components:{
        Myhero,
        stickyHeader,
        cards,
        aboutNetwork,
        businessArea,
        pricing,
        news,
        newsletter,
        message,

    },
    data(){
        return{
            headerData : [
                {
                    name: 'HOME',

                },
                {
                    name: 'ABOUT',
                    
                },
                {
                    name: 'SERVICES',
                   
                },
                {
                    name: 'PRICING',
                   
                },
                {
                    name: 'BLOG',
                    
                },
                {
                    name: 'GET IN TOUCH',
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