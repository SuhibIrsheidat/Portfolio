<template>
    <div id="Gallery" class="Compartment">
        <div class="compInfo">
            <div class="compTitle">Gallery</div>
            <br><br>
            <SlideShow/>
        </div>
    </div>
</template>

<script>
import SlideShow from './SlideShow.vue'

export default {
    name: 'Gallery',
    components: {
        SlideShow
    }
}
</script>

<style>
</style>