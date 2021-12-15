<template>
  <div id="app">
    <Myheader />
    <Mymain />
    <Myfooter :footerElements="this.footerData"/>
  </div>
</template>
<script>
import Myheader from './components/Myheader.vue'
import Mymain from './components/Mymain.vue'
import Myfooter from './components/Myfooter.vue'
export default {
  name: 'App',
  components: {
    Myheader,
    Mymain,
    Myfooter
  },

  data(){
        return{
            footerData: [
                {
                    title: 'About',
                    links: [
                        {
                            name: 'The Company'
                        },
                        {
                            name: 'Institutional'
                        },
                        {
                            name: 'Social & Events'
                        },
                        {
                            name: 'Innovation'
                        },
                        {
                            name: 'Environment'
                        },
                        {
                            name: 'Technologyy'
                        },
                    ]
                },
                {
                    title: 'Services',
                    links: [
                        {
                            name: 'Audit & Assurance'
                        },
                        {
                            name: 'Financial Advisory'
                        },
                        {
                            name: 'Analytics M&A'
                        },
                        {
                            name: 'Middle Marketing'
                        },
                        {
                            name: 'Legal Consulting'
                        },
                        {
                            name: 'Regulatory Risk'
                        },
                    ]
                },
                {
                    title: 'Support',
                    links: [
                        {
                            name: 'Responsability'
                        },
                        {
                            name: 'Terms of use'
                        },
                        {
                            name: 'About Cookies'
                        },
                        {
                            name: 'Privacy Policy'
                        },
                        {
                            name: 'Accessibility'
                        },
                        {
                            name: 'Information'
                        },
                    ]
                },
            ]
        }
    }

}
</script>

<style lang="scss">
   *{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
    } 
    @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@900&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap');
</style>

