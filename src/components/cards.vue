<template>
    <div class="cards-container">
        <div class="cards-centered">
            <div class="card">
                <div class="card-icon">
                    <div class="icon-bg"></div>
                    <i class="far fa-user fa-2x"></i>
                </div>
                <h2>Human Capital</h2>
                <p>Humanizing business: Harness the power of technology to improve the way people work</p>
            </div>
            <div class="card">
                <div class="card-icon">
                    <div class="icon-bg"></div>
                    <i class="fas fa-chart-pie fa-2x"></i>
                </div>
                <h2>Core Business</h2>
                <p>It takes innovative approaches to transform, modernize, and run existing platforms</p>
            </div>
            <div class="card">
                <div class="card-icon">
                    <div class="icon-bg"></div>
                    <i class="fas fa-tachometer-alt fa-2x"></i>
                </div>
                <h2>Performance</h2>
                <p>Achieving maximum impact and value from investmens in finance and supply chain</p>
            </div>
        </div>    
    </div>
</template>

<script>
export default {
    name : 'cards'
}
</script>

<style lang="scss">
.cards-container{
    background-color: #e3e7df;
    display: flex;
    justify-content: center;
    color: black;
    padding: 3rem 0;
    
    .cards-centered{
        width: 75%;
        display: flex;
        .card{
            background-color: #ffffff;
            width: calc(100% / 3);
            padding: 2rem;
            margin: 0 0.5rem;
            border-radius: 5px;
            position: relative;
            top: 0;
            transition: all 0.3s;
            h2{
                margin: 1.5rem 0;
            }
            .card-icon{
                position: relative;
                width: 70px;
                height: 70px;
                text-align: center;
                line-height: 70px;
                .icon-bg{
                    background-color: #0d7e7e;
                    filter: opacity(0.5);
                    position: absolute;
                    height: 100%;
                    width: 100%;
                    border-radius: 50%;
                }
                i{
                    color: #0d7e7e;
                    padding: 1rem;
                }
            } 
            
            &:hover{
                top: -10px;
            }
        }
    }
}
@media screen and (max-width: 1215px) {
    .cards-centered{
        width: 95% !important;
    }
}
</style>
