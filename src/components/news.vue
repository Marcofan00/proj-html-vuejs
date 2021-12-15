<template>
    <div class="news-container">
        <div class="news-centered">
            <p class="green">OUR EDITORIAL CONTENT</p>
            <div class="news-title">
                <div class="title-left">
                    <h1>Latest</h1>
                </div>
                <div class="title-right">
                    <div class="title-bg"></div>
                    <h1 class="absolute">News</h1>
                    <h1 class="hidden">News</h1>
                </div>
            </div>
            <div class="news-text">
                <p>Every Week we publish content about what is best in the business world</p>
                <button class="btn">SEE ALL</button>
            </div>
            <div class="news-cards">
                <div class="card">
                    <div class="card-child bg-1"></div>
                    <div class="blurred-bg"></div>
                    <h3>Increasing creativity is possible for everyone</h3>
                    <p class="bottom">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    <div class="top">
                        <div class="user">
                            <i class="far fa-user"></i>
                            <p>Andrea Miller</p>
                        </div>
                        <div class="date">
                            <i class="far fa-clock"></i>
                            <p>2 Days Ago</p>
                        </div>
                    </div>
                </div>
                <div class="card middle">
                    <div class="card-child bg-2"></div>
                    <div class="blurred-bg"></div>
                    <h3>Because market research is bart of the business plan</h3>
                    <p class="bottom">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    <div class="top">
                        <div class="user">
                            <i class="far fa-user"></i>
                            <p>Andrea Miller</p>
                        </div>
                        <div class="date">
                            <i class="far fa-clock"></i>
                            <p>2 Days Ago</p>
                        </div>
                    </div>
                </div>
                <div class="card">
                    <div class="card-child bg-3"></div>
                    <div class="blurred-bg"></div>
                    <h3>Working from home is now a trend</h3>
                    <p class="bottom">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    <div class="top">
                        <div class="user">
                            <i class="far fa-user"></i>
                            <p>Andrea Miller</p>
                        </div>
                        <div class="date">
                            <i class="far fa-clock"></i>
                            <p>2 Days Ago</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
name : 'news'
}
</script>

<style lang="scss">
.news-container{
    display: flex;
    justify-content: center;
    padding: 5rem 0;
    .news-centered{
        width: 75%;
        .green{
            color: #0d7e7e;
            margin-bottom: 0.5rem;
        }
        .news-title{
            display: flex;
            margin-bottom: 1rem;
            .title-left{
                color: #1e2223;
            }
            .title-right{
                position: relative;
                .title-bg{
                    height: 100%;
                    width: 100%;
                    background-color: #0d7e7e;
                    filter: opacity(0.3);
                }
                .absolute{
                    position: absolute;
                    top: 0;
                    color: #0d7e7e;
                    padding-left: 0.5rem;
                }
                .hidden{
                    visibility: hidden;
                    padding: 0 0.5rem;
                }
            }
        }
        .news-text{
            display: flex;
            justify-content: space-between;
            margin-bottom: 2rem;
            p{
                color: #1e2223;
            }
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
        }
        .news-cards{
            width: 100%;
            height: 420px;
            display: flex;
            
            .card{
                width: calc(100% / 3);
                height: 100%;
                overflow: hidden;
                position: relative; 
                display: flex;
                justify-content: center;
                border-radius: 30px;
                background-position: center;
                .card-child{
                    background-size: cover;
                    height: 100%;
                    width: 100%;
                    display: flex;
                    align-items: center;
                    filter: brightness(0.4);
                    transition: all 0.3s;
                    transform: none;
                }
                .blurred-bg{
                    backdrop-filter: blur(0);
                    position: absolute;
                    height: 100%;
                    width: 100%;
                    top: 0;
                    transition: all 0.3s;
                }
                .bg-1{
                    background-image: url('../assets/news-1.jpg');
                }
                .bg-2{
                    background-image: url('../assets/news-2.jpg');
                }
                .bg-3{
                    background-image: url('../assets/news-3.jpg');
                }
                h3{
                    position: absolute;
                    bottom: 10%;
                    padding: 0 1.5rem;
                    text-align: center;
                    transition: all 0.3s;
                }
                .bottom{
                    bottom: 0;
                    transition: all 0.3s;
                    position: absolute;
                    opacity: 0;
                    transition: all 0.3s;
                    padding: 0 2rem;
                    text-align: center;
                }
                .top{
                    top: 0;
                    transition: all 0.3s;
                    position: absolute;
                    display: flex;
                    justify-content: space-around;
                    width: 100%;
                    padding: 0 1.5rem;
                    opacity: 0;
                    .date, .user{
                        display: flex;
                        align-items: center;
                        i{
                            margin-right: 0.5rem;
                        }
                    }
                }
                &:hover{
                    cursor: pointer;
                
                    .card-child{
                        transform: scale(1.3);
                        filter: brightness(0.4);
                        box-shadow: 0;
                        margin: -10px;
                    }
                    .blurred-bg{
                        backdrop-filter: blur(3px);
                    }
                    h3{
                        bottom: 20%;
                    }
                    .bottom{
                        bottom: 10%;
                        opacity: 1;
                    }
                    .top{
                        top: 10%;
                        opacity: 1;
                    }
                }
            }
            
            .middle{
                margin: 0 1.5rem;
                display: flex;
                justify-content: center;
            }
        }
    }
}
@media screen and (max-width: 1215px) {
    .news-centered{
        width: 95% !important;
        .news-cards{
            height: 300px !important;
            h3{
                font-weight: 100 !important;
                font-size: medium;
                
            }
            .card:hover{
                h3{
                    bottom: 25% !important;
                }
            }
        }
    }
}
</style>