<template>
    <div>
        <section id="contact">
            <div class="contact--container">
                <div class="contact--information">
                    <div class="contact--detail"><span class="fa fa-envelope"></span></div>
                    <div class="contact--detail"><span class="fab fa-whatsapp"></span></div>
                    <div class="contact--detail"><span class="fa fa-phone"></span></div>
                    <div class="contact--detail"><span class="fab fa-instagram"></span></div>
                    <div class="contact--detail"><span class="fab fa-github"></span></div>
                    <div class="contact--detail"><span class="fab fa-twitter"></span></div>
                    <div class="contact--detail"><span class="fab fa-telegram"></span></div>
                </div>
                <div class="copyright">&copy; Rafiu Olakunle Moshood {{ (new Date()).getFullYear() }}</div>
            </div>
        </section>
    </div>
</template>
<script>
export default {
    
}
</script>
<style>
    #contact{
        height: 40vh;
        background: #fff;
        color: #000;
        position: relative;
    }
    .contact--container{
        position: absolute;
        top: 60%;
        left: 50%;
        width: 100%;
        transform: translateX(-50%)translateY(-50%);
    }
    .contact--information{
        display: flex;
        justify-content: center;
    }
    .contact--information .contact--detail{
        padding: 20px;
        font-size: 30px;
        cursor: pointer;
    }
    .copyright{
        text-align: center;
        letter-spacing: 1px;
    }
    @media screen and (max-width: 700px) {
        .contact--information .contact--detail{
            padding: 15px;
            font-size: 25px;
        }
    }
    @media screen and (max-width: 500px) {
        .contact--information .contact--detail{
            padding: 12px;
            font-size: 20px;
        }
    }
    @media screen and (max-width: 370px) {
        .contact--information .contact--detail{
            padding: 10px;
            font-size: 16px;
        }
    }
</style>