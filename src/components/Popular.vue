<template>
	<section class="popular">
		<!-- <div class="planner__input">
	        <svg class="planner__icon" 
				 width="561px" height="561px" viewBox="0 0 561 561" style="enable-background:new 0 0 561 561;" xml:space="preserve">
				<g>
					<g id="gps-fixed">
						<path d="M280.5,178.5c-56.1,0-102,45.9-102,102c0,56.1,45.9,102,102,102c56.1,0,102-45.9,102-102
							C382.5,224.4,336.6,178.5,280.5,178.5z M507.45,255C494.7,147.9,410.55,63.75,306,53.55V0h-51v53.55
							C147.9,63.75,63.75,147.9,53.55,255H0v51h53.55C66.3,413.1,150.45,497.25,255,507.45V561h51v-53.55
							C413.1,494.7,497.25,410.55,507.45,306H561v-51H507.45z M280.5,459C181.05,459,102,379.95,102,280.5S181.05,102,280.5,102
							S459,181.05,459,280.5S379.95,459,280.5,459z"/>
					</g>
				</g> 
			</svg>
			<input type="text" placeholder="Starting point">
			<div class="planner__dest">
					Starting point
				</div>
		</div> -->
		<router-link to="/popular" class="planner__inputlink">
			<div class="planner__input"> 
				<svg class="planner__icon" 
					 width="510px" height="510px" viewBox="0 0 510 510" style="enable-background:new 0 0 510 510;" xml:space="preserve">
					<g>
						<g id="place">
							<path d="M255,0C155.55,0,76.5,79.05,76.5,178.5C76.5,311.1,255,510,255,510s178.5-198.9,178.5-331.5C433.5,79.05,354.45,0,255,0z
								 M255,242.25c-35.7,0-63.75-28.05-63.75-63.75s28.05-63.75,63.75-63.75s63.75,28.05,63.75,63.75S290.7,242.25,255,242.25z"/>
						</g>
					</g>
				</svg> 
				<div class="planner__dest">
					Where do you want to go?
				</div>
		        
	        </div>
        </router-link>
		<h1 class="popular__title headtitle">Most popular</h1>

		<div class="planner-popular">

			<flickity ref="flickity" :options="flickityOptions">
			<div class="planner-popular__item pp1 planner__rijksmuseum clickie">
				<router-link to="/rijksmuseum">
				<div class="planner-popular__img">
					<div class="planner-popular__text">
						
							<h2 class="planner-popular__title" @click="preview">Rijksmuseum</h2>
						
						<div class="planner-popular__distance">Museum</div>
					</div>
				</div>
				</router-link>
			</div>

			<div class="planner-popular__item pp2 planner__vangogh clickie">
				<div class="planner-popular__img">
					<div class="planner-popular__text">
						<router-link to="/vangogh">
							<h2 class="planner-popular__title">Van Gogh Museum</h2>
						</router-link>
						<div class="planner-popular__distance">Museum</div>
					</div>
				</div> 
			</div>

			<div class="planner-popular__item pp3 planner__anne">
				<div class="planner-popular__img">
					<div class="planner-popular__text">
						<router-link to="#">
							<h2 class="planner-popular__title">Anne Frank House</h2>
						</router-link>
						<div class="planner-popular__distance">Museum</div>
					</div>
				</div> 
			</div>

			<div class="planner-popular__item pp2 planner__artis clickie">
				<router-link to="/artis">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							
								<h2 class="planner-popular__title" @click="preview">Artis</h2>
							
							<div class="planner-popular__distance">Zoo</div>
						</div>
					</div>
				</router-link> 
			</div>

			<div class="planner-popular__item pp2 planner__brouwerij clickie">
				<div class="planner-popular__img">
					<div class="planner-popular__text">
						<router-link to="/heineken">
							<h2 class="planner-popular__title">Heineken Experience</h2>
						</router-link>
						<div class="planner-popular__distance">Old brewery</div>
					</div>
				</div> 
			</div>

			<div class="planner-popular__item pp2 planner__stedelijk">
				<div class="planner-popular__img">
					<div class="planner-popular__text">
						<router-link to="#">
							<h2 class="planner-popular__title">Stedelijk Museum</h2>
						</router-link>
						<div class="planner-popular__distance">Museum</div>
					</div>
				</div> 
			</div>

			<div class="planner-popular__item pp2 planner__nemo">
				<div class="planner-popular__img">
					<div class="planner-popular__text">
						<router-link to="#">
							<h2 class="planner-popular__title">Nemo</h2>
						</router-link>
						<div class="planner-popular__distance">Science Museum</div>
					</div>
				</div> 
			</div>

			<div class="planner-popular__item pp2 planner__eye">
				<div class="planner-popular__img">
					<div class="planner-popular__text">
						<router-link to="#">
							<h2 class="planner-popular__title">Eye</h2>
						</router-link>
						<div class="planner-popular__distance">Filmmuseum</div>
					</div>
				</div> 
			</div>

			<div class="planner-popular__item pp2 planner__herm">
				<div class="planner-popular__img">
					<div class="planner-popular__text">
						<router-link to="#">
							<h2 class="planner-popular__title">Hermitage</h2>
						</router-link>
						<div class="planner-popular__distance">Museum</div>
					</div>
				</div> 
			</div>
			
			<div class="planner-popular__item pp2 planner__scheepe">
				<div class="planner-popular__img">
					<div class="planner-popular__text">
						<router-link to="#">
							<h2 class="planner-popular__title">National Maritime Museum</h2>
						</router-link>
						<div class="planner-popular__distance">Museum</div>
					</div>
				</div> 
			</div>

			</flickity>

		</div>

		<h1 class="popular__title exploretitle">Explore Amsterdam By Theme</h1>
		<h1 class="popular__title exploretitle blacktitle">Food</h1>
		<div class="planner-popular">
			<flickity ref="flickity" :options="flickityOptions">
				<div class="planner-popular__item pp4 planner__boiboi">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview">Boi Boi</h2>
							</router-link>
							<div class="planner-popular__distance">Thai</div>
						</div>
					</div>
				</div>

				<div class="planner-popular__item pp5 planner__rijsel">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview">Rijsel</h2>
							</router-link>
							<div class="planner-popular__distance">French-Flemish</div>
						</div>
					</div>
				</div>

				<div class="planner-popular__item pp6 planner__505">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview">Vijfnulvijf</h2>
							</router-link>
							<div class="planner-popular__distance">Asian fusion</div>
						</div>
					</div>
				</div>

				<div class="planner-popular__item pp6 viewmore">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview">View more</h2>
							</router-link>
							
						</div>
					</div>
				</div>
			</flickity>
		</div>

		<h1 class="popular__title exploretitle blacktitle">10 of the best wine bars</h1>
		<div class="planner-popular">
			<flickity ref="flickity" :options="flickityOptions">
				<div class="planner-popular__item pp7 planner__vyne">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview">Vyne</h2>
							</router-link>
							<!-- <div class="planner-popular__distance">2.1km</div> -->
						</div>
					</div>
				</div>

				<div class="planner-popular__item pp8 planner__glou">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview">Glou Glou</h2>
							</router-link>
							<!-- <div class="planner-popular__distance">1.2km</div> -->
						</div>
					</div>
				</div>

				<div class="planner-popular__item pp9 planner__wester">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview">Wester Wijnfabriek</h2>
							</router-link>
							<!-- <div class="planner-popular__distance">500m</div> -->
						</div>
					</div>
				</div>
				<div class="planner-popular__item pp6 viewmore">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview">View more</h2>
							</router-link>
							
						</div>
					</div>
				</div>
			</flickity>
		</div>

		<h1 class="popular__title exploretitle blacktitle">5 things to do in Noord</h1>
		<div class="planner-popular tempimg">
			<flickity ref="flickity" :options="flickityOptions">
				<div class="planner-popular__item pp6 viewmore">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview"></h2>
							</router-link>
							
						</div>
					</div>
				</div>

				<div class="planner-popular__item pp6 viewmore">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview"></h2>
							</router-link>
							
						</div>
					</div>
				</div>

				<div class="planner-popular__item pp6 viewmore">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview"></h2>
							</router-link>
							
						</div>
					</div>
				</div>
				<div class="planner-popular__item pp6 viewmore">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview"></h2>
							</router-link>
							
						</div>
					</div>
				</div>
			</flickity>
		</div>

		<h1 class="popular__title exploretitle blacktitle">5 things to do in Oostelijke Eilanden</h1>
		<div class="planner-popular tempimg">
			<flickity ref="flickity" :options="flickityOptions">
				<div class="planner-popular__item pp6 viewmore">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview"></h2>
							</router-link>
							
						</div>
					</div>
				</div>

				<div class="planner-popular__item pp6 viewmore">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview"></h2>
							</router-link>
							
						</div>
					</div>
				</div>

				<div class="planner-popular__item pp6 viewmore">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview"></h2>
							</router-link>
							
						</div>
					</div>
				</div>
				<div class="planner-popular__item pp6 viewmore">
					<div class="planner-popular__img">
						<div class="planner-popular__text">
							<router-link to="#">
								<h2 class="planner-popular__title" @click="preview"></h2>
							</router-link>
							
						</div>
					</div>
				</div>
			</flickity>
		</div>

	</section>
</template>

<script>
	import { eventBus } from '../main';
	import Flickity from 'vue-flickity';

	export default {
		data: function() {
	        return {
	            destination: 'Where to?',
	            flickityOptions: {
	                // initialIndex: 1,
	                prevNextButtons: false,	
	                pageDots: false,
	                //wrapAround: false,
	                autoPlay: false,
	                cellAlign: 'left',
	                contain: true

	                // any options from Flickity can be used
	            }
	        }
	    }, 
	    components: {
	        Flickity
	    },
		props: { 
			userAge: String
		},
		methods: { 
			preview() {
				this.myName = "preview";
				this.$emit('nameWasReset1', this.myName);
				this.inOut = "in-out";
				this.$emit('modusInOut', this.inOut);
			}
		},
		created() { 
		},
		mounted () { 
	      const tlVueGsap = new TimelineMax()
	        .from('.pp1', 0.7, {y: 100, autoAlpha:0, ease: Power4.easeOut} )
	        .from('.pp2', 0.7, {y: 100, autoAlpha:0, ease: Power4.easeOut}, '-=0.5')
	        .from('.pp3', 0.7, {y: 100, autoAlpha:0, ease: Power4.easeOut}, '-=0.5')

	        .from('.pp4', 0.7, {y: 100, autoAlpha:0, ease: Power4.easeOut}, '-=0.7')
	        .from('.pp5', 0.7, {y: 100, autoAlpha:0, ease: Power4.easeOut}, '-=0.5')
	        .from('.pp6', 0.7, {y: 100, autoAlpha:0, ease: Power4.easeOut}, '-=0.5')

	        .from('.pp7', 0.7, {y: 100, autoAlpha:0, ease: Power4.easeOut}, '-=0.5')
	        .from('.pp8', 0.7, {y: 100, autoAlpha:0, ease: Power4.easeOut}, '-=0.5')
	        .from('.pp9', 0.7, {y: 100, autoAlpha:0, ease: Power4.easeOut}, '-=0.5')

	        .from('.headtitle', 0.5, {autoAlpha:0, ease: Power4.easeOut}, 0.2)
	        .from('.exploretitle', 0.6, {autoAlpha:0, ease: Power4.easeOut}, 0.3)
	    }
	} 
	
</script>

<style lang="scss" scoped> 

	h1 {
		font-size: 1.25em;
		margin: 0;
		font-weight: 600;
    	margin-bottom: 0.5em;
	}
	.blacktitle {
		color: #659fff;
		font-size: 1em;
	}
	.headtitle {
		margin-top: 1em;
	}
	.popular {
		background-color: #fff;
		overflow-x: hidden;
		height: 100vh;
		&__title {
			padding: 0 1rem;
		}
		// .popular__title,
		// .planner-popular {
		// 	opacity: 0;
		// 	animation: fadein 0.75s cubic-bezier(0.785, 0.135, 0.15, 0.86) forwards;
		// }
	}

	@keyframes fadein {
		0% {
			//opacity: 0;
		}
		100% {
			opacity: 1;
		}
	}
	.planner {
		overflow: hidden;
		&__input {
			width: calc(100% - 4em);
			padding: 1em;
			margin: 0 auto;
			background-color: #fff;
			z-index: 2;
			position: relative;
			box-shadow: 0 0.25em 1em 0 rgba(0,0,0,0.15);
		}
		&__icon {
			width: 0.8em;
			height: 1em;
			fill: #757575;
			position: relative;
			opacity: 0.5;
			display: inline-block;
			top: 3px;
    		left: -3px;
		} 
		&__dest {
			display: inline-block;
			color: #9e9e9e;
		}
		&__rijksmuseum {
			.planner-popular__img {
				background-image: url('../assets/rijksmuseum.jpg');
			}
		}
		&__vangogh {
			.planner-popular__img {
				background-image: url('../assets/vangogh.jpg');
			}
		}
		&__anne {
			.planner-popular__img {
				background-image: url('../assets/annefrank.jpg');
			}
		}
		&__stedelijk {
			.planner-popular__img {
				background-image: url('../assets/stedelijk.jpg');
			}
		}
		&__nemo {
			.planner-popular__img {
				background-image: url('../assets/nemo.jpg');
			}
		}
		&__eye {
			.planner-popular__img {
				background-image: url('../assets/eye.jpg');
			}
		}
		&__herm {
			.planner-popular__img {
				background-image: url('../assets/hermitage.jpg');
			}
		}
		&__scheepe {
			.planner-popular__img {
				background-image: url('../assets/scheep.jpg');
			}
		}
		&__boiboi {
			.planner-popular__img {
				background-image: url('../assets/boiboi.jpg');
			}
		}
		&__rijsel {
			.planner-popular__img {
				background-image: url('../assets/rijsel.jpg');
			}
		}
		&__505 {
			.planner-popular__img {
				background-image: url('../assets/505.jpg');
			}
		}
		&__vyne {
			.planner-popular__img {
				background-image: url('../assets/vyne.jpg');
			}
		}
		&__glou {
			.planner-popular__img {
				background-image: url('../assets/glou.jpg');
			}
		}
		&__wester {
			.planner-popular__img {
				background-image: url('../assets/wester.jpg');
			}
		}
		&__artis {
			.planner-popular__img {
				background-image: url('../assets/artis.jpg');
				background-position: center center;
			}
		}
		&__heineken {
			.planner-popular__img {
				background-image: url('../assets/brouwerij.jpg');
			}
		}
		&__brouwerij {
			.planner-popular__img {
				background-image: url('../assets/heineken.jpg');
			}
		}
		&__dappermarkt {
			.planner-popular__img {
				background-image: url('../assets/dappermarkt.jpg');
			}
		}
		&__javastraat {
			.planner-popular__img {
				background-image: url('../assets/javastraat.jpg');
			}
		}
		&__scheep {
			.planner-popular__img {
				background-image: url('../assets/scheeps.jpg');
			}
		}
		
	} 
	.planner-popular {
		//overflow-x: hidden; 
		//padding-bottom: 2em;
		//display: flex;
		//width: 100em;
		&__item {   
			box-shadow: 0 0.25em 1em 0 rgba(0,0,0,0.15);
			border-radius: 0.2em;
			margin: 0 0 2em 1em;
			display: inline-block;
			width: 150px;
		}
		&__info {
			padding: 0.75em 0.5em;
		}
		&__title {
			font-size: 1rem;
			font-weight: 900;
			margin: 0;
			color: #fff;

		}
		&__text {
			padding: 0.75em 0.5em 0.3em;
			position: absolute;
			bottom: 0;
			z-index: 1;
		}
		&__distance {
			color: #fff;
			font-size: 0.75em;
		}
		&__img {
			height: 10em;
			background-size: cover;
			position: relative;
			&:after {
				position: absolute;
				content:"";
				top:0;
				left:0;
				width:100%;
				height:100%;
				opacity:0.75;
				background: linear-gradient(to bottom, rgba(0,0,0,0) 41%,rgba(0,0,0,0.59) 76%,rgba(0,0,0,1) 100%);
			}
		}
		
	}
	.clickie {
		.planner-popular__img:after {
			border-bottom: 4px rgba(0, 0, 255, 0.3) solid;
		}
	}
	.viewmore {
		&:after {
			position: absolute;
			content:"";
			top:0;
			left:0;
			width:100%;
			height:100%;
			opacity:0.75;
			background-color: #000;
		}
		.planner-popular__text {
			bottom: 20%;
		    left: 20%;
		}
	}
	.tempimg {
		.viewmore {
			&:after {
				position: absolute;
				content:"";
				top:0;
				left:0;
				width:100%;
				height:100%;
				opacity:0.75;
				background-color: #2979ff;
			}
			.planner-popular__text {
				bottom: 20%;
			    left: 20%;
			}
		}
	}
	input {
		border: 0;
		border-bottom: 0.063em solid #e0e0e0;
		width: calc(100% - 10em);
		padding: 0.5em 0;
		&::placeholder {
			font-size: 1.2em;
		}
	}
</style>