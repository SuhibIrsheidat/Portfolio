<template>
    <div class="galleryWindow">
        <button class="slideButton" id="slideLeft" @click="slideLeft()">
            <i class="fa fa-angle-left"></i>
        </button>
        <button class="slideButton" id="slideRight" @click="slideRight()">
            <i class="fa fa-angle-right"></i>
        </button>
        <div class="slide" id="slide-1">
            <img src="@/assets/images/slideShow/slide-1.png"/>
            <div>
                Augmented Reality Maps
                <div style="font-size: 0.75vw; margin-top: 2vw; letter-spacing: 2px; font-family: Sora-Regular">
                    MADE TO INTRODUCE THE ROLE OF <b>AR</b> IN REALIFE SCENARIOS
                </div>
                <br><br>
                <button class="galleryButton">
                    Project Available upon Request
                </button>
            </div>
        </div>
        <div class="slide" id="slide-2">
            <img src="@/assets/images/slideShow/slide-2.png"/>
            <div>
                Financial Oragnizer
                <div style="font-size: 0.75vw; margin-top: 2vw; letter-spacing: 2px; font-family: Sora-Regular">
                    Organize your cards and payments in <b>one place</b>
                </div>
                <br><br>
                <button class="galleryButton">
                    Project Available upon Request
                </button>
            </div>
        </div>
        <div class="slide" id="slide-3">
            <img src="@/assets/images/slideShow/slide-3.png"/>
            <div>
                Music player
                <div style="font-size: 0.75vw; margin-top: 2vw; letter-spacing: 2px; font-family: Sora-Regular">
                    Enjoy listening to music with <b>Adaptive waves</b> in your seek bar
                </div>
                <br><br>
                <button class="galleryButton">
                    Project Available upon Request
                </button>
            </div>
        </div>
        <div class="slide" id="slide-4">
            <img src="@/assets/images/slideShow/slide-4.png"/>
            <div>
                Furniture Inventory
                <div style="font-size: 0.75vw; margin-top: 2vw; letter-spacing: 2px; font-family: Sora-Regular">
                    Shop your house furniture in <b>the simpliest way</b> of shopping
                </div>
                <br><br>
                <button class="galleryButton">
                    Project Available upon Request
                </button>
            </div>
        </div>
        <div class="slide" id="slide-5">
            <img src="@/assets/images/slideShow/slide-5.png"/>
            <div>
                Forecast application
                <div style="font-size: 0.75vw; margin-top: 2vw; letter-spacing: 2px; font-family: Sora-Regular">
                    Stay dry with <b>User friendly</b> forecast application
                </div>
                <br><br>
                <button class="galleryButton">
                    Project Available upon Request
                </button>
            </div>
        </div>
        <div class="slide" id="slide-6">
            <img src="@/assets/images/slideShow/slide-6.png"/>
            <div>
                Chatting application
                <div style="font-size: 0.75vw; margin-top: 2vw; letter-spacing: 2px; font-family: Sora-Regular">
                    connect with people is now <b>seamlessly easy</b> 
                </div>
                <br><br>
                <button class="galleryButton">
                    Project Available upon Request
                </button>
            </div>
        </div>
        <div class="slide" id="slide-7">
            <img src="@/assets/images/slideShow/slide-7.png"/>
            <div>
                BiFitness Health Application
                <div style="font-size: 0.75vw; margin-top: 2vw; letter-spacing: 2px; font-family: Sora-Regular">
                    Monitor your workouts and <b>earn badges</b> with BiFitness
                </div>
                <br><br>
                <button class="galleryButton">
                    Project Available upon Request
                </button>
            </div>
        </div>
    </div>
</template>

<script>
var slideCount = 1
var slides = []

export default {
    name: 'SlideShow',
    mounted: function () {
        this.$nextTick(function () {
            slides.push(document.getElementById('slide-1'))
            slides.push(document.getElementById('slide-2'))
            slides.push(document.getElementById('slide-3'))
            slides.push(document.getElementById('slide-4'))
            slides.push(document.getElementById('slide-5'))
            slides.push(document.getElementById('slide-6'))
            slides.push(document.getElementById('slide-7'))
            slides.forEach(slide => {
                if (slide.id.includes('-' + slideCount)){
                    slide.style.display = 'flex'
                } else {
                    slide.style.display = 'none'
                }
            })
        })
    },
    methods: {
        showAndHide: function () {
            slides.forEach(slide => {
                if (slide.id.includes('-' + slideCount)){
                    slide.style.display = 'flex'
                } else {
                    slide.style.display = 'none'
                }
            })
        },
        slideRight: function(){
            slideCount += 1
            if (slideCount > 7)
                slideCount = 1
            this.showAndHide()
        },
        slideLeft: function(){
            slideCount -= 1
            if (slideCount < 1)
                slideCount = 7
            this.showAndHide()
        }
    }
}
</script>

<style>
.galleryWindow{
    width: 75vw;
    height: 70vh;
    position: relative;
}

.slideButton{
    background: unset;
    border: none;
    color: #f0f0f0;
    font-size: 4vw;
    cursor: pointer;
    transition: 0.25s all;
}

.slideButton:hover{
    transform: scale(1.3);
    transition: 0.25s all;
}

#slideLeft{
    position: absolute;
    top: 29vh;
}

#slideRight{
    position: absolute;
    top: 29vh;
    right: 0
}

.slide{
    width: 60vw;
    height: 70vh;
    margin-left: 7.25vw;
    position: relative;
    display: flex;
    flex-direction: row;
    align-self: center;
    align-items: center;
    transition: 0.25s all;
}

.slide img:nth-child(1) {
    height: 100%;
    transition: 0.25s all;
}

.slide img:hover{
    transform: scale(1.05);
    transition: 0.25s all;

}

.slide div:nth-child(2){
    letter-spacing: 5px;
    margin-left: 4vw;
    font-family: Sora-Bold;
    font-size: 1.75vw;
}

.galleryButton{
    background: unset;
    border: 1px solid #40A4FF;
    font-family: Sora-Regular;
    color: #40A4FF;
    padding: 1vw 3vw;
    letter-spacing: 4px;
    border-radius: 2vw;
    font-size: 0.85vw;
    transition: 0.25s all;
}
</style>