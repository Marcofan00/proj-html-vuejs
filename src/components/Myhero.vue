<template>
    <div class="hero-container">
        <div class="hero-background">
            <img src="../assets/hero-image.png" alt="">
        </div>
            <div class="hero-content">
                <div class="title">
                    <h1>Lead</h1>
                    <h1 class="space">~</h1>
                    <div class="customer-container">
                        <div class="customer-bg"></div>
                        <h1>Customer</h1>
                    </div>
                </div>
                <div class="text">
                    <p>Succesful strategies require data analysis, creatifity and customer focus, taking 
                        advantage of the latest technologies to offer excellent services.</p>   
                </div>   
                <div class="hero-buttons-container">
                    <button class="btn">GET IN TOUCH</button>
                    <button class="btn border">READ MORE</button>    
                </div> 
            </div>
        
    </div>
</template>

<script>
export default {
    name : 'Myhero',
}
</script>

<style lang="scss">

.hero-container{
    height: calc(100vh - 30px);
    display: flex;
    justify-content: center;
    position: relative;
    overflow: hidden;
    
    .hero-background{
      filter: brightness(0.4);
      background-size: cover;
     

    }

    .hero-content{
        position: absolute;
        top: 35%;
        display: flex;
        flex-direction: column;
        align-items: center;
        font-size: large;
        width: 60%;
        height: 30%;
        .title{
            display: flex;
            position: relative;
            color: #ffffff;
            font-weight: 900;
            font-size: xx-large;
            
            .space{
                margin-left:1rem;
                margin-right: 0.5rem;
            }
            .customer-container{
                position: relative;
                h1{
                    padding: 0 0.5rem;
                }
                .customer-bg{
                    position: absolute;
                    background-color: #0d7e7e;
                    height: 100%;
                    width: 100%;
                    filter: opacity(0.1);
                    text-align: center;
                }
            }
        }
        .text{
            text-align: center;
            color: #a2adae;
            margin-top: 2rem;
            font-size: x-large;
            font-weight: 900;
        }
        .hero-buttons-container{
            height: 50px;
            margin-top: 2rem;
            .btn{
                margin: 0 1rem;
                border: 0;
                font-weight: 900;
                font-size: medium;
                color: white; 
                padding: 0.75rem 1rem;  
                border: 2px solid #0d7e7e;
                border-radius: 3px;
                background-color: #0d7e7e;
                line-height: 100%;
                transition: all 0.3s;
            }
            .border{
                border: 2px solid #0d7e7e;
                background-color: transparent ;
                &:hover{
                    background-color: #0d7e7e;
                }
            }
        }
    }
}
</style>