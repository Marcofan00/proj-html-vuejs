<template>
    <div class="header">
        <div class="info-contacts">
            <div class="left-contacts">
              <i class="fas fa-clock"></i>
              <p>Open Hour: Mon - Sat - 9:00 - 18:00</p>
            </div>
            <div class="right-contacts">
                <div class="phone-number">
                    <i class="fas fa-phone-alt"></i>
                    <p>+1 (305) 1234-5678</p>
                </div>
                <div class="mail-contact">
                    <i class="fas fa-envelope"></i>
                    <p>hello@example.com</p>
                </div>
                <div class="social-pages">
                    <i class="fab fa-facebook-f"></i>
                    <i class="fab fa-twitter"></i>
                    <i class="fab fa-linkedin-in"></i>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:'Myheader',
}
</script>

<style lang="scss">
.header{
    background-color: #24333d;
    color: #e3e7df;
    height: 50px;
    line-height: 50px;
    display: flex;
    justify-content: center;
    .info-contacts{
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 75%;
        .left-contacts{
            display: flex;
            align-items: center;
        }
        .right-contacts{
            display: flex;
            div{
                display: flex;
                align-items: center;
                margin: 0 1rem;
            }
            .social-pages{
                margin-right: 0;
                
                i{
                    margin: 0 1rem;
                }
            }
        }
        i{
            margin: 0 0.5rem;
        }
    }
}
@media screen and (max-width: 1215px) {
    .info-contacts-container{
        width: 95% !important;
    }
}
</style>
