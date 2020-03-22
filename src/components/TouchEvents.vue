<template>
    <section>
        <h1>vue2-touch-events</h1>

        <div class="carousel" v-touch:swipe="swipeHandler" v-touch:tap="tapHandler">
            <div>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Delectus laudantium, minima molestias odit
                perferendis repellendus.
            </div>
            <div>Culpa deserunt dignissimos dolorem ea eius in iste iure nesciunt placeat, quidem quisquam quos
                veritatis?
            </div>
            <div>Alias culpa debitis dignissimos, dolorum ea eveniet harum inventore ipsa ipsam quam quos reiciendis
                velit?
            </div>
            <div>Dolorum ipsa labore odio, odit quibusdam quos tempore totam vitae. Alias autem dolores itaque nulla?
            </div>
            <div>Cum, laboriosam vitae. Aut consequatur cum distinctio id inventore ipsa ipsam laborum quae sequi
                temporibus?
            </div>
            <div>At atque, error eum nesciunt omnis quia quos repudiandae. Animi dolore incidunt placeat sequi?
                Dolore.
            </div>
            <div>Amet aut beatae consectetur cumque distinctio eaque modi, nisi officia quos, recusandae repudiandae
                unde veritatis!
            </div>
            <div>Aliquam dolorem error nam nostrum recusandae sit veniam! Aliquid animi assumenda dicta, itaque nisi
                sit?
            </div>
            <div>Ad ex facilis libero, magni minima nihil nobis officia officiis optio qui, sed velit veniam!</div>
        </div>
    </section>
</template>

<script>
	export default {
		name: "TouchEvents",
		methods: {
			swipeHandler (e) {
				console.log('swipe: ',e)
			},
			tapHandler (e) {
				console.log('tap: ',e)
			}
		},
	}
</script>

<style scoped>
    .carousel {
        display: flex;
        width: 100%;
        overflow: hidden;
        flex-direction: row;
    }

    .carousel > div {
        flex: 1 0 100px;
        background: darkgreen;
        color: white;
    }
</style>