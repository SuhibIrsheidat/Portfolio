<template>
    <div class="nav-list">
        <a href="#Experience">
            <button class="navButton">Experience</button>
        </a>
        <a href="#Education">
            <button class="navButton">Education</button>
        </a>
        <a href="#Gallery">
            <button class="navButton">Gallery</button>
        </a>
        <a href="#Skills">
            <button class="navButton">Skills</button>
        </a>
        <a href="#Contact">
            <button class="navButton">Contact</button>
        </a>
    </div>
</template>

<script>
export default {
    name: 'Navigation'
}
</script>

<style>
.nav-list{
    width: 60vw;
    height: 8vh;
    display: flex;
    flex-direction: row;
    align-items: center;
    align-self: center;
    justify-content: space-around;
    margin: auto;
}

.navButton{
    width: 10.5vw;
    font-size: 0.75vw;
    padding: 0.5vw 1.25vw;
    background: unset;
    border-top: 1px solid #0000;
    border-left: 1px solid #0000;
    border-right: 1px solid #0000;
    border-bottom: 1px solid #fff4;
    border-radius: 0vw;
    color: white;
    font-family: Sora-Regular;
    letter-spacing: 2px;
    cursor: pointer;
    text-align: center;
    transition: 0.5s all;
}

.navButton:hover{
    border: 1px solid #E12179;
    border-radius: 2vw;
    letter-spacing: 3px;
    transition: 0.25s all;
}

</style>