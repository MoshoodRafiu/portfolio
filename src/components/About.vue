<template>
    <div>
        <section id="about">
            <div class="col-md-6 about--item image--section">
                <div class="about--item-content">
                    <img src="../assets/about.svg" width="100%" alt="icon">
                </div>
            </div>
            <div class="col-md-6  about--item">
                <div class="about--item-content">
                    <div class="about--section-header">
                        <h3>About Me</h3>
                        <div class="underline">
                            <div class="underline-start"></div>
                            <div class="underline-end"></div>
                        </div>
                    </div>
                    <div class="about--section-content">
                        <p>
                            I am a creative and ambitious web developer and programmer with a talent for critical reasoning, problem solving
                        and time management.I am currently in my fourth year of studying Electronic and Computer Engineering at Lagos
                        state University. I have excellent communication skills, enabling me to effectively communicate with a wide range
                        of people and I am eager to be challenged so as to develop and also improve my skills. My passion is to provide
                        solutions to problems that in turn benefits both individuals and organizations.
                        </p>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>
<script>
export default {
    name: 'about'
}
</script>
<style>
    #about{
        height: 100vh;
        display: flex;
    }
    .about--item{
        height: 100vh;
        position: relative;
    }
    .about--item
    .about--item-content{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateX(-50%)translateY(-50%);
    }
    .about--item-content
    .about--section-header h3{
        font-size: 40px;
        text-transform: uppercase;
    }
    .about--item-content
    .about--section-content p{
        padding: 10px 0;
        font-size: 17px;
        letter-spacing: 1px;
        word-spacing: 5px;
    }
    .underline{
        display: flex;
    }
    .underline-start,
    .underline-end{
        height: 3px;
        background: #000;
    }
    .underline-start{
        width: 80px;
    }
    .underline-end{
        width: 30px;
        margin-left: 10px;
    }
    @media screen and (max-width: 780px) {
        .about--item.image--section{
            display: none;
        }
    }
</style>