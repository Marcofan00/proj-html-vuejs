<template>
    <div class="about-container">
        <div class="about-left">
            <div class="about-content">
                <p class="green">ABOUT THE NETWORK</p>
                <div class="about-title">
                    <div class="title-left">
                        <div class="title-bg"></div>
                        <h1>The</h1>
                    </div>
                    <div class="title-right">
                        <h1>Company</h1>
                    </div>
                </div>
                <div class="about-text">
                    <p>For 12 years we have been providing audit and warranty, financial
                        advice, risk, taxes and related services to select clients.
                    </p>
                </div>
                <div class="about-cards">
                    <div class="row">
                        <div class="card">
                            <div class="card-title">
                                <i class="fas fa-medal fa-lg"></i>
                                <h2>Tradition</h2>
                            </div>    
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        </div>
                        <div class="card">
                            <div class="card-title">
                                <i class="fas fa-lock fa-lg"></i>
                                <h2>Security</h2>
                            </div>
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        </div>
                    </div>
                    <div class="row">
                        <div class="card"> 
                            <div class="card-title">
                                <i class="fas fa-edit fa-lg"></i>
                                <h2>Certificate</h2>
                            </div>    
                            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        </div>
                        <div class="card">
                            <div class="card-title">
                                <i class="fas fa-graduation-cap fa-lg"></i>
                                <h2>Expertise</h2>
                            </div>    
                            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="about-right">
            
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style lang="scss">
.about-container{
    display: flex;
    position: relative;
    .about-left{
        width: 50%;
        height: 100%;
        display: flex;
        justify-content: right;
        padding: 5rem 0;
        .about-content{
            width: 75%;
            
            .green{
                color: #0d7e7e;
                margin-bottom: 1rem;
            }
            .about-title{
                display: flex;
                margin-bottom: 1rem;
                .title-left{
                    position: relative;
                    color: #0d7e7e;
                    .title-bg{
                        position: absolute;
                        height: 100%;
                        width: 100%;
                        background-color: #0d7e7e;
                        filter: opacity(0.3);
                        border-radius: 3px;
                    }
                    
                    h1{
                        padding: 0 0.5rem;
                    }
                }
                .title-right{
                    color: #1e2223;
                }
            }
            
            .about-text{
                color: #778a94;
                margin-bottom: 3rem;
            }
            .about-cards{
                color: #778a94;
                .row{
                    display: flex;
                    margin-bottom: 2rem;
                    .card{
                        width: 50%;
                        padding-right: 1rem 0;
                        .card-title{
                            display: flex;
                            align-items: center;
                            h2{
                                margin-left: 0.5rem;
                                color: #1e2223;
                            }
                        }
                        i{
                            color: #0d7e7e;
                        }
                        p{
                            margin: 2rem 0
                        };
                    }
                }
            }
        }
    }
    .about-right{
        width: 50%;
        background-image: url('../assets/about-3.jpg');
        background-position: center;
        padding: 5rem 0;
        background-size: cover;
    }
}
@media screen and (max-width: 1215px) {
    .about-content{
        width: 97.5% !important;
    }
}
</style>