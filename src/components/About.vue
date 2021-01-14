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
    .underline{
        display: flex;
    }
    .underline-start,
    .underline-end{
        height: 3px;
        background: #000;
    }
    .underline-start{
        width: 70px;
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