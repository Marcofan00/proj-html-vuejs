<template>
    <div class="pricing-container">
        <div class="pricing-centered">
            <div class="pricing-content">
                <p class="green">MONTLY PLANS</p>
                <div class="pricing-title">
                    <div class="title-left">
                        <div class="title-bg"></div>
                        <h1 class="hidden">Pricing</h1>
                        <h1 class="absolute">Pricing</h1>
                    </div>
                    <div class="title-right">
                        <h1>Table</h1>
                    </div>
                </div>
                <div class="pricing-text">
                    <p>We can help you deliver and execute your future, wherever you compete, using the latest
                        technologies, from strategy development to implementation.
                    </p>
                </div>
            </div>
            <div class="pricing-cards">
                <div class="card">
                    <div class="card-arrow">
                        <div class="arrow-bg"></div>
                        <i class="fas fa-arrow-right fa-2x hidden"></i>
                        <i class="fas fa-arrow-right fa-2x absolute"></i>
                    </div>
                    <i class="fas fa-rocket fa-2x"></i>
                    <h3>Standard</h3>
                    <div class="price">
                        <p>$</p>
                        <h2>490</h2>
                        <p>/ MO</p>
                    </div>
                    <div class="features">
                        <div class="feature">
                            <p>Standard Accounting</p>
                            <i class="fas fa-check"></i>
                        </div>
                        <div class="feature">
                            <p>Platform Access</p>
                            <i class="fas fa-check"></i>
                        </div>
                        <div class="feature">
                            <p>Business Orientation</p>
                            <i class="fas fa-times"></i>
                        </div>
                        <div class="feature">
                            <p>Dedicated Consultant</p>
                            <i class="fas fa-times"></i>
                        </div>
                        <div class="feature">
                            <p>Personal Assistance</p>
                            <i class="fas fa-times"></i>
                        </div>
                    </div>
                </div>
                <div class="card popular">
                    <div class="bigger-background">
                        <div class="card-arrow">
                            <div class="arrow-bg"></div>
                            <i class="fas fa-arrow-right fa-2x hidden"></i>
                            <i class="fas fa-arrow-right fa-2x absolute"></i>                  
                        </div>
                    </div>               
                    <div class="card-content">
                        <div class="most-popular">
                            <p>Most</p>
                            <p>Popular</p>
                        </div>
                        <i class="fas fa-briefcase fa-2x"></i>
                        <h3>Professional</h3>
                        <div class="price">
                            <p>$</p>
                            <h2>890</h2>
                            <p>/ MO</p>
                        </div>
                        <div class="features">
                            <div class="feature">
                                <p>Standard Accounting</p>
                                <i class="fas fa-check"></i>
                            </div>
                            <div class="feature">
                                <p>Platform Access</p>
                                <i class="fas fa-check"></i>
                            </div>
                            <div class="feature">
                                <p>Business Orientation</p>
                                <i class="fas fa-check"></i>
                            </div>
                            <div class="feature">
                                <p>Dedicated Consultant</p>
                                <i class="fas fa-times"></i>
                            </div>
                            <div class="feature">
                                <p>Personal Assistance</p>
                                <i class="fas fa-times"></i>
                            </div>
                        </div>
                    </div>    
                </div>
                <div class="card">
                    <div class="card-arrow">
                        <div class="arrow-bg"></div>
                        <i class="fas fa-arrow-right fa-2x hidden"></i>
                        <i class="fas fa-arrow-right fa-2x absolute"></i>
                    </div>
                    <i class="far fa-gem fa-2x"></i>
                    <h3>Ultimate</h3>
                    <div class="price">
                        <p>$</p>
                        <h2>1.390</h2>
                        <p>/ MO</p>
                    </div>
                    <div class="features">
                        <div class="feature">
                            <p>Standard Accounting</p>
                            <i class="fas fa-check"></i>
                        </div>
                        <div class="feature">
                            <p>Platform Access</p>
                            <i class="fas fa-check"></i>
                        </div>
                        <div class="feature">
                            <p>Business Orientation</p>
                            <i class="fas fa-check"></i>
                        </div>
                        <div class="feature">
                            <p>Dedicated Consultant</p>
                            <i class="fas fa-check"></i>
                        </div>
                        <div class="feature">
                            <p>Personal Assistance</p>
                            <i class="fas fa-check"></i>
                        </div>
                    </div>
                </div> 
            </div>    
        </div>
    </div>
</template>

<script>
export default {
    name: 'pricing'
}
</script>

<style lang="scss">
.pricing-container{
    display: flex;
    justify-content: center;
    background-color: #e3e7df;
    padding: 8rem 0;
    .pricing-centered{
        width: 75%;
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        
        .pricing-content{
            text-align: center;
            width: 75%;
            margin-bottom: 1rem;
            .green{
                color: #0d7e7e;
                margin-bottom: 0.5rem;
            }
            .pricing-title{
                display: flex;
                justify-content: center;
                margin-bottom: 1rem;
                .title-left{
                    position: relative;
                    padding: 0 0.5rem;
                    
                    .title-bg{
                        height: 100%;
                        width: 100%;
                        background-color: #0d7e7e;
                        filter: opacity(0.3);
                    }
                    .hidden{
                        visibility: hidden;
                        position: relative;
                        top: 0;
                        padding: 0 0.5rem;
                    }
                    .absolute{
                        position: absolute;
                        top: 0;
                        color: #0d7e7e;
                        padding-left: 0.5rem;
                    }
                }
                .title-right{
                    color: #1e2223;
                }
            }
            .pricing-text{
                color: #778a94;
                margin-bottom: 2rem;
            }
        }
        .pricing-cards{
            width: 100%;
            display: flex;
            .card{
                width: calc(100% / 3);
                padding: 5rem 2rem;
                background-color: #ffffff;
                display: flex;
                flex-direction: column;
                align-items: center;
                border-radius: 10px;
                transition: all 0.3s;
                position: relative;
                top: 0;
                .card-arrow{
                    color: #0d7e7e;
                    margin: 1rem;
                    position: absolute;
                    top: 0;
                    right: 0;
                    .arrow-bg{
                        background-color: #0d7e7e;
                        height: 0;
                        width: 0;
                        top: 50%;
                        left: 50%;
                        position: absolute;
                        border-radius: 50%;
                        transition: all 0.7s linear;
                    }
                    .hidden{
                        visibility: hidden;
                    }
                    .absolute{
                        position: absolute;
                        top: 0;
                        left: 0;
                        color: #0d7e7e;
                        opacity: 0;
                        transition: opacity 0.3s;
                    }
                }
                i{
                    color: #0d7e7e;
                }
                h3{
                    color: #1e2223;
                    margin: 1rem 0;
                }
                .price{
                    color: #0d7e7e;
                    display: flex;
                    align-items: baseline;
                    margin-bottom: 2rem;
                    justify-content: center;
                    h2{
                        margin: 0 0.25rem;
                        font-size: xx-large;
                    }
                }
                .features{
                    width: 100%;
                    display: flex;
                    flex-direction: column;
                    .feature{
                        display: flex;
                        width: 100%;
                        justify-content: space-between;
                        margin-bottom: 1rem;
                        i{
                            width: 5%;
                            text-align: center;
                        }
                        p{
                            color: #1e2223;
                        }
                    }
                } 
                
                &:hover{
                    top: -10px;   
                    .arrow-bg{
                        animation: display  0.7s;
                    }
                    .absolute{
                        opacity: 1;
                    }
                }
            }
            .popular{
                position: relative;
                margin: 0 1rem;
                text-align: center;
                .most-popular{
                    position: absolute;
                    background-color: #0d7e7e;
                    top: 5%;
                    left: 0;
                    padding-right: 1.5rem;
                    padding-left: 0.5rem;
                    border-top-right-radius: 30px;
                    border-bottom-right-radius: 30px;
                    font-weight: 900;
                    color: white;              
                }
                .bigger-background{
                    position: absolute;
                    height: 110%;
                    width: 100%;
                    padding: 4rem;
                    top: -5%;
                    background-color: white;
                    border-radius: 10px;
                }
                .card-content   {
                    z-index: 2;
                    width: 100%;
                }
            }
        }
    }
}
@media screen and (max-width: 1215px) {
    .pricing-centered{
        width: 95% !important;
    }
}
</style>