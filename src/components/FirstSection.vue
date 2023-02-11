<template>
    <section id="home" class="banner slide-bg relative z-0 pb-16 pt-32 overflow-hidden before:opacity-90 before:w-full before:h-full before:z-0 before:absolute before:top-0 before:left-0 h-auto lg:h-[800px]">
			<!-- Container -->
			<div class="container max-w-7xl w-full mx-auto md:px-6 lg:px-10 px-1">
				<div class="row items-center flex flex-wrap -mr-1 -ml-1">
					<!-- Content -->
					<div class="res-margin relative z-20 w-full px-4 text-left max-w-full md:max-w-[58.333333%] lg:max-w-[50%] mb-8 md:mb-0 lg:mb-0">
						<!-- Banner text -->

							<h1 class="wow fadeInUp  text-white font-roboto font-bold  tracking-tight mb-6  leading-[1.2] text-4xl md:text-[3.75rem] lg:text-6xl text-tighter md:text-tight lg:text-tight text-center lg:text-left" data-wow-offset="10" data-wow-duration="1s" data-wow-delay="0s" style="visibility: visible; animation-duration: 1s; animation-delay: 0s; animation-name: fadeInUp;">
								Get the new App for <br>iPhone &amp; Android
							</h1>
							
							<p class="wow fadeInUp text-white mb-10 text-lg text-center lg:text-left leading-[1.75]" data-wow-offset="10" data-wow-duration="1s" data-wow-delay="0.3s" style="visibility: visible; animation-duration: 1s; animation-delay: 0.3s; animation-name: fadeInUp;">
								Mauris ut fermentum orci. 
								Pellentesque ultrices interdum ultrices. 
								Aliquam erat volutpat. 
								Mauris molestie aliquam hendrerit. 
								Integer cursus neque eget auctor finibus, at enim euismod.
							</p>

							<div data-wow-offset="10" data-wow-duration="1s" data-wow-delay="0.6s" style="visibility: visible; animation-duration: 1s; animation-delay: 0.6s; animation-name: fadeInUp;">
								
								<a href="#" class="py-2.5 px-2.5 md:px-4 lg:px-4 m-2 border-white border-solid border font-medium rounded inline-flex mr-2.5">
									<BellIcon class="h-5 w-5 text-2xl mt-1 text-white font-normal inline-block mr-2.5" aria-hidden="true" /><p><span class=" block text-white font-bold text-lg">Google Play</span></p>
								</a>
								
								<a href="#" class="py-2.5 px-2.5 md:px-4 lg:px-4 min-w-[150px] m-2 border-white border-solid border font-medium rounded inline-flex">
									<BellIcon class="h-5 w-5 text-2xl mt-1 text-white font-normal inline-block mr-2.5" aria-hidden="true" /><p><span class=" block text-white font-bold text-lg">App Store</span></p>
								</a>
							
							</div>

					
					</div>  
					
					<!-- Image -->
					<div class="relative w-full z-20 max-w-full md:max-w-[41.666%] lg:max-w-[50%] px-4 lg:px-0">
						<div class="banner-image-center wow fadeInUp relative my-0 mx-auto text-center max-w-full lg:max-w-[300px]" data-wow-offset="10" data-wow-duration="1s" data-wow-delay="0.3s" style="visibility: visible; animation-duration: 1s; animation-delay: 0.3s; animation-name: fadeInUp;">
							<img src="slide-welcome.png">
						</div>

					</div>
					
				</div>
				
			</div>
			
			<!-- Bottom shape -->
            <div class="bottom-shape absolute z-10 top-auto -bottom-1 left-0 right-0">
                <svg viewBox="0 0 1920 310" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" class="svg replaced-svg">
                    <g stroke="none" stroke-width="1" fill="none" fill-rule="evenodd">
                        <g transform="translate(0.000000, -554.000000)" fill="#fafbfe">
                            <path d="M-3,551 C186.257589,757.321118 319.044414,856.322454 395.360475,848.004007 C509.834566,835.526337 561.525143,796.329212 637.731734,765.961549 C713.938325,735.593886 816.980646,681.910577 1035.72208,733.065469 C1254.46351,784.220361 1511.54925,678.92359 1539.40808,662.398665 C1567.2669,645.87374 1660.9143,591.478574 1773.19378,597.641868 C1848.04677,601.75073 1901.75645,588.357675 1934.32284,557.462704 L1934.32284,863.183395 L-3,863.183395"></path>
                        </g>
                    </g>
                </svg>
            </div>
			
            <div class="backstretch top-0 left-0 overflow-hidden m-0 p-0 -z-10 absolute w-screen" style="height: 800px">
                <img class="absolute m-0 p-0 border-none w-screen max-h left-0 -top-4" src="slideshow-2.jpg">
            </div>
    </section>
</template>


<script setup>
import { Bars3Icon, BellIcon, XMarkIcon } from '@heroicons/vue/24/outline';
</script>