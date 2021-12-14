<template>
	<div class="stickyheader-container" :class="{nav_colored: scrollPosition > 50}">
		<div class="nav-container">
		<div class="nav-left">
			<div class="logo-container">
			<div class="left-logo">
				<div class="background-logo"></div>
				<h1>NEX</h1>
			</div>
			<div class="right-logo">
				<h1>GEN</h1>
			</div>
			</div>
		</div>
		<div class="nav-right">
			<a v-for="element in headerElements" :key="element.id" :class="element.class" :id="element.id">{{element.name}}</a>
		</div>
		</div>
	</div>
</template>

<script>
export default {
  name: "stickyHeader",
    data() {
        return{
            scrollPosition: null
        }
    },
	props:{
		headerElements: Array
	},
    mounted() {
        window.addEventListener('scroll', this.updateScroll);
		let home = document.getElementById('scrollHome')
		home.addEventListener('click', this.scrollHome)
        let about = document.getElementById('scrollAbout')
        about.addEventListener('click', this.scrollAbout)
        let services = document.getElementById('scrollServices')
        services.addEventListener('click', this.scrollServices)
        let pricing = document.getElementById('scrollPricing')
        pricing.addEventListener('click', this.scrollPricing)
        let blog = document.getElementById('scrollBlog')
        blog.addEventListener('click', this.scrollBlog)
        let touch = document.getElementById('scrollTouch')
        touch.addEventListener('click', this.scrollTouch)
    },
    methods: {
        updateScroll() {
            this.scrollPosition = window.scrollY
        },
		scrollHome(){
			window.scrollTo(0, document.getElementById('home').offsetTop-0);
		},
        scrollAbout(){
            window.scrollTo(0, document.getElementById('about').offsetTop-30);
        },
        scrollServices(){
            window.scrollTo(0, document.getElementById('services').offsetTop-30);
        },
        scrollPricing(){
            window.scrollTo(0, document.getElementById('pricing').offsetTop-30);
        },
        scrollBlog(){
            window.scrollTo(0, document.getElementById('blog').offsetTop-30);
        },
        scrollTouch(){
            window.scrollTo(0, document.getElementById('touch').offsetTop-30);
        }
    }   
};
</script>

<style lang="scss">

.stickyheader-container{
	display: flex;
	justify-content: center;
	position: sticky;
	top: -1px;
	z-index: 3;
	width: 100%;
	transition: all 0.3s;
	background-color: transparent;
	.nav-container{
		display: flex;
		justify-content: space-between;
		width: 75%;
		height: 50px;
		z-index: 1;
		align-items: center;
		margin: 1rem 0;
		.nav-left{
			.logo-container{
				display: flex;
				font-weight: 900;
				align-items: center;
				.left-logo{
                    color: #0d7e7e;
					position: relative;
					display: flex;
					padding-left: 1.5rem;
					font-weight: 900;
					
					.background-logo{
						position: absolute;
						height: 100%;
						width: 100%;
						background-color: #0d7e7e;
						filter: opacity(0.3);
						left: 0;
						border-top-left-radius: 25px;
						border-bottom-left-radius: 25px;
					}
					h1{
						padding-right: 0.5rem;
					}
				}
			}
		}
		.nav-right{
			display: flex;
			align-items: center;
			height: 100%;
			a{
				text-decoration: none;
				color: #e3e7df;
				padding: 0 1rem;
				font-weight: 900;
				cursor: pointer;
				&:hover{
					color: #0d7e7e;
				}
			}
			.btn{
				padding: 0.75rem 1rem;
				color: #e3e7df !important;
				text-align: center;
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
	}
}
@media screen and (max-width: 1215px) {
    .nav-container{
		width: 95% !important;
	}
}
</style>