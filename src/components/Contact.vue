<template>
    <div id="Contact" class="Compartment">
        <div class="compInfo">
            <div class="compTitle">Personal Details</div>
            <br>
            <div class="pill">
                &bull; Full Name: <b>Suhib Ahmad Irsheidat</b>
            </div>
            <div class="pill">
                &bull; Birthday: <b>04 February 1997</b>
            </div>
            <div class="pill">
                &bull; Nationality: <b>Jordanian</b>
            </div>
            <div class="pill">
                &bull; Languages: <b>Arabic - English - German</b>
            </div>
            <br><br><br><br>
            <div class="compTitle">Contact</div>
            <br>
            <div class="pill">
                &bull; Email: <b>SUHIBBASHA@GMAIL.com</b>
            </div>
            <div class="pill">
                &bull; Phone Number: <b>+962 781 500 907</b>
            </div>
            <div class="pill">
                &bull; LinkedIn: 
                <a href="https://www.linkedin.com/in/suhaib-irsheidat-822883163/" target="_blank">
                    Suhib Irsheidat
                </a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Contact'
}
</script>

<style>
.pill{
    width: auto;
    padding: 1vw 2vw;
    color: #40A4FF;
    letter-spacing: 2px;
    font-size: 1vw;
}

.pill b{
    color: #f0f0f0;
}

a{
    color: #f0f0f0;
    text-decoration: underline;
    font-weight: bold;
}
</style>