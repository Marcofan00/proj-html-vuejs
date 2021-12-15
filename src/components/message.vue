<template>
    <div class="message-container">
        <div class="message-centered">
            <div class="message-left">
                <p class="green">SEND MESSAGE</p>
                <div class="message-title">
                    <div class="title-left">
                        <h1>Get in</h1>
                    </div>
                    <div class="title-right">
                        <div class="title-bg"></div>
                        <h1 class="hidden">Touch</h1>
                        <h1 class="absolute">Touch</h1>
                    </div>
                </div>
                <div class="message-text">
                    <p>We will respond to your message as soon as possible.</p>
                </div>
                <div class="message-form">
                    <form action="#">
                        <div class="iconed">
                            <input name="name" type="text" placeholder="Name">
                            <img src="../assets/image (1).png" alt="">
                        </div>
                        <input name="mail" type="email" placeholder="Email">
                        <input name="phone" type="text" placeholder="Phone">
                        <select name="selection" value="selection">
                            <option value="">More Info</option>
                            <option value="">lorem </option>
                            <option value="">lorem</option>
                            <option value="">lorem</option>
                            <option value="">lorem</option>
                            <option value="">lorem</option>
                        </select>   
                        <input class="message" name="message" type="text" placeholder="Message">
                        <button class="btn">SEND</button>
                    </form>
                </div>
            </div>
            <div class="message-right">
                <h3>Example Inc.</h3>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                <p>Present diam lacus,dapibus sed imperdiet consectetur.</p>
                <div class="contacts-container">
                    <div class="contact">
                        <div class="icon">
                            <div class="icon-bg"></div>
                            <i class="fas fa-phone-alt fa-lg"></i>
                        </div>   
                        <p>+1 (305) 1234-5678</p>
                    </div>
                    <div class="contact">
                        <div class="icon">
                            <div class="icon-bg"></div>
                            <i class="fas fa-envelope fa-lg"></i>
                        </div>   
                        <p>Hello@example.com</p>
                    </div>
                    <div class="contact">
                        <div class="icon">
                            <div class="icon-bg"></div>
                            <i class="fas fa-map-marker-alt fa-lg"></i>
                        </div>    
                        <p>Main Avenue, 987</p>
                    </div>
                    <button class="btn">VIEW MAP</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name : 'message',
    data() {
        return{
            selection:""
        }
    }
}
</script>

<style lang="scss">
.message-container{
    display: flex;
    justify-content: center;
    padding: 7rem 0;
    .message-centered{
        width: 75%;
        display: flex;
        .message-left{
            width: 70%;
            
            .green{
                color: #0d7e7e;
                margin-bottom: 1rem;
            }
            .message-title{
                display: flex;
                margin-bottom: 2rem;
                .title-left{
                    color: #24333d;
                }
                .title-right{
                    position: relative;
                    .title-bg{
                        background-color: #0d7e7e;
                        filter: opacity(0.3);
                        height: 100%;
                        width: 100%;
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
            .message-text{
                
                p{
                    color: #24333d;
                    margin-bottom: 2rem;
                }
            }
            .message-form{
                form{
                    display: flex;
                    flex-wrap: wrap;
                    justify-content: space-between;
                    input,select{
                        width: 49%;
                        padding: 0.5rem;
                        background-color: #e3e7df;
                        border: 0;
                        margin-bottom: 1rem;
                        border-radius: 3px;
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
                    .iconed{
                        position: relative;
                        width: 49%;
                        display: flex;
                        align-items: center;
                        margin-bottom: 1rem;
                        input{
                            width: 100%;
                            margin-bottom: 0;
                        }
                        img{
                            position: absolute;
                            right: 0;
                            padding: 0.25rem;
                        }
                        i{
                            position: absolute;
                            right: 2%;
                            align-self: center;
                            color: #24333d;
                            filter: opacity(0.5);
                        }
                    }
                    .message{
                        width: 100%;
                        padding-bottom: 5rem;
                    }
                }
            }
        }
        .message-right{
            width: 30%;
            padding-left: 1.5rem;
            display: flex;
            flex-direction: column;
            justify-content: center;
            h3,p{
                color: #24333d;
                margin-bottom: 1rem;
            }
            .contacts-container{
                width: 100%;
                .contact{
                    display: flex;
                    width: 100%;
                    align-items: center;
                    margin-bottom: 1rem;
                    p{
                        margin-bottom: 0;
                    }
                    .icon{
                        position: relative;
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        margin-right: 0.5rem;
                        .icon-bg{
                            height: 50px;
                            width: 50px;
                            background-color: #0d7e7e;
                            filter: opacity(0.3);
                            text-align: center;
                            line-height: 50px;
                            border-radius: 50%;
                            position: relative;
                        }
                        i{
                            color: #0d7e7e;
                            z-index: 2;
                            position: absolute;
                        }
                    }    
                }
            }
            .btn{
                 margin: 0 1rem;
                border: 0;
                font-weight: 900;
                font-size: medium;
                color: #0d7e7e; 
                padding: 0.75rem 1rem;  
                border: 2px solid #0d7e7e;
                border-radius: 3px;
                background-color: transparent;
                line-height: 100%;
                transition: all 0.3s;
                &:hover{
                    background-color: #0d7e7e !important;
                    color: white;
                }
            }
        }
    }
}
@media screen and (max-width: 1215px) {
    .message-centered{
        width: 95% !important;
    }
}
</style>