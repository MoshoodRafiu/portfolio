<template>
    <div>
        <section id="contact">
            <div class="contact--container">
                <div class="contact--information">
                    <div class="contact--detail"><a target="_blank" href="https://facebook.com/moshood.rafiu.1"><span class="fab fa-facebook-f"></span></a></div>
                    <div class="contact--detail"><a target="_blank" href="tel:2348144259341"><span class="fa fa-phone"></span></a></div>
                    <div class="contact--detail"><a target="_blank" href="https://www.instagram.com/devkunle"><span class="fab fa-instagram"></span></a></div>
                    <div class="contact--detail"><a target="_blank" href="https://github.com/MoshoodRafiu"><span class="fab fa-github"></span></a></div>
                    <div class="contact--detail"><a target="_blank" href="https://twitter.com/devrom_"><span class="fab fa-twitter"></span></a></div>
                    <div class="contact--detail"><a target="_blank" href="mailto:rafiumoshoodolakunle@gmail.com"><span class="fa fa-envelope"></span></a></div>
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
        height: 30vh;
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
    .contact--information .contact--detail a{
        color: #000;
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