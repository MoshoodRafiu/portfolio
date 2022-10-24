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
                            <div class="underline-container">
                                <div class="underline-start"></div>
                                <div class="underline-end"></div>
                            </div>
                        </div>
                    </div>
                    <div class="about--section-content">
                        <p>
                            An innovative software engineer with a 5-year Computer Engineering degree and 2 years of experience. Well-versed
                            in technology and writing code to develop software that is reliable and user-friendly. A creative tech
                            enthusiast with a talent for critical reasoning and problem-solving, and a passion to contribute to how the
                            internet is progressing and how technology is evolving.
                        </p>
                    </div>
                    <div class="about--section-footer">
                        <a href="./Moshood Rafiu CV.pdf" download>Download CV</a>
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
        min-height: 100vh;
        display: flex;
    }
    .about--item{
        min-height: 100vh;
        position: relative;
    }
    .about--item
    .about--item-content{
        position: absolute;
        top: 50%;
        left: 50%;
        width: 80%;
        transform: translateX(-50%)translateY(-50%);
    }
    .about--item-content
    .about--section-header h3{
        font-size: 35px;
        text-transform: uppercase;
    }
    .about--item-content
    .about--section-content p{
        padding: 10px 0;
        font-size: 15px;
        letter-spacing: 1px;
        word-spacing: 5px;
        font-family: 'Noto Sans TC', sans-serif;
    }
    .about--item-content
    .about--section-footer a{
        padding: 10px;
        width: 150px;
        font-size: 15px;
        text-transform: uppercase;
        border: none;
        background: transparent;
        color: #000;
        border: 1px solid #000;
        letter-spacing: 3px;
        text-decoration: none;
    }
    .about--item-content
    .about--section-footer a:hover{
        background: #000;
        color: #fff;
    }
    .underline{
        display: flex;
        margin-bottom: 20px;
        width: 100%;
    }
    .underline-start,
    .underline-end{
        height: 3px;
        background: #000;
    }
      .underline-container{
            display: flex;
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
        .about--item-content
        .about--section-header h3{
            text-align: center;
        }
        .underline-container{
            margin: auto;
        }
    }
</style>