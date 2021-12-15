<template>
    <div class="footer-container">
        <div class="footer-content">
            <div class="content-centered">
                <div class="footer-col">
                    <div class="footer-title">
                        <div class="title-left">
                            <div class="title-bg"></div>
                            <h1 class="hidden">NEX</h1>
                            <h1 class="absolute">NEX</h1>
                        </div>
                        <div class="title-right">
                            <h1>GEN</h1>
                        </div>
                    </div>    
                    <div class="col-text">
                        <p>A Functional HTML Template for Corporate & Business.</p>
                    </div>
                    <div class="contacts-container">
                        <div class="contact">
                            <div class="icon">
                                <i class="fas fa-phone-alt fa-lg"></i>
                            </div>   
                            <p>+1 (305) 1234-5678</p>
                        </div>
                        <div class="contact">
                            <div class="icon">
                                <i class="fas fa-envelope fa-lg"></i>
                            </div>   
                            <p>Hello@example.com</p>
                        </div>
                        <div class="contact">
                            <div class="icon">
                                <i class="fas fa-map-marker-alt fa-lg"></i>
                            </div>    
                            <p>Main Avenue, 987</p>
                        </div>
                        <button class="btn">GET IN TOUCH</button>
                    </div>           
                </div>
                <div v-for="element in footerElements" :key="element.title" class="footer-col effect">
                    <div class="col-title"> 
                        <h2>{{element.title}}</h2>
                    </div>    
                    <div v-for="el in element.links" :key="el.link" class="link-container">
                        <i class="fas fa-angle-right"></i>
                        <a href="#">{{el.name}}</a>
                    </div> 
                </div>
            </div>
        </div>
        <div class="footer-privacy">
            <div class="privacy-centered">
                <p>Enjoy the low price. We are tracking any intention of piracy.</p>
                <div class="privacy-right">
                    <p>© 2020 NEXGEN is Proudly powered by&nbsp;</p>
                    <a href="#">Codings</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'Myfooter',
    props:{
        footerElements: Array
    }
}
</script>

<style lang="scss">
.footer-container{
    .footer-content{
        display: flex;
        justify-content: center;
        background-color: #121117;
        color: white;
        padding: 7rem 0;
        .content-centered{
            width: 75%;
            display: flex;
            .footer-col{
                width: 25%;
                margin: 0 0.75rem;
                background-color: #1e2223;
                padding: 2rem;
                border-radius: 15px;
                
                .btn{
                    margin: 0 1rem;
                    border: 0;
                    font-weight: 900;
                    font-size: medium;
                    color: white; 
                    padding: 0.75rem 1rem;  
                    border: 2px solid #0d7e7e;
                    border-radius: 3px;
                    line-height: 100%;
                    transition: all 0.3s;
                    background-color: transparent;
                    &:hover{
                        background-color: #0d7e7e;
                    }
                }
                .footer-title{
                    display: flex;
                    margin-bottom: 1rem;
                    .title-left{
                        position: relative;
                        .title-bg{
                            height: 100%;
                            width: 100%;
                            background-color: #0d7e7e;
                            border-top-left-radius: 25px;
                            border-bottom-left-radius: 25px;
                            filter: opacity(0.5);
                        }
                        .hidden{
                            visibility: hidden;
                            padding-left: 2rem;
                        }
                        .absolute{
                            position: absolute;
                            color: #0d7e7e;
                            top: 0;
                            padding-left: 1.5rem;
                        }
                    }
                }
                .col-text{
                    margin-bottom: 1rem;
                }
                .contacts-container{
                    
                    .contact{
                        display: flex;
                        width: 100%;
                        margin-bottom: 1rem;
                        .icon{
                            width: 10%;
                            display: flex;
                            align-items: center;
                            justify-content: center;
                        }
                        &:hover{
                            color: #0d7e7e;
                            cursor: pointer;
                        }
                    }
                }
                .col-title{
                    margin-bottom: 1rem;
                }
                .link-container{
                    display: flex;
                    margin-bottom: 1rem;
                    align-items: center;
                    i{
                        margin-right: 0.5rem;
                    }
                    &:hover{
                        color: #0d7e7e;
                        cursor: pointer;
                        a{
                            color: #0d7e7e;
                        }
                    }
                }
            }
            .footer-col:first-of-type{
                margin-left: 0;
                background-color: transparent;
                padding-left: 0;
            }
            .footer-col:last-of-type{
                margin-right: 0;
            }
            .effect{
                position: relative;
                top: 0;
                transition: all 0.3s;
                a{
                    text-decoration: none;
                    color: white;
                }
                &:hover{
                    top: -10px;
                }
            }
        }
    }
    .footer-privacy{
        display: flex;
        justify-content: center;
        background-color: #25262e;
        padding: 1rem 0;
        color: white;
        .privacy-centered{
            width: 75%;
            display: flex;
            justify-content: space-between;
            .privacy-right{
                display: flex;
                a{
                    color: #0d7e7e;
                    text-decoration: none;
                    &:hover{
                        text-decoration: underline;
                    }
                }
            }
        }
    }
}
@media screen and (max-width: 1215px) {
    .content-centered, .privacy-centered{
        width: 95% !important;
        .footer-col{
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
    }
}
</style>