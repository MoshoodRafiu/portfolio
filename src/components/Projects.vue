<template>
    <div>
        <section id="projects">
            <div class="projects--container">
                <div class="projects--container-content">
                    <div class="projects--section-header">
                        <h3>Projects</h3>
                        <div class="underline mx-auto">
                            <div class="mx-auto d-flex">
                                <div class="underline-start light"></div>
                                <div class="underline-end light"></div>
                            </div>
                        </div>
                    </div>
                    <div class="projects--section-header">
                        <div class="row">
                            <div class="col-lg-4 col-md-6">
                                <div class="project--container">
                                    <div class="project--header">
                                        Project Name
                                    </div>
                                    <div class="project--body">
                                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ratione mollitia illum ullam autem eos, tempore illo consequatur aperiam iste nostrum!
                                    </div>
                                    <div class="project--footer">
                                        <img src="../assets/techs/html.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/css.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/javascript.svg" class="project--footer-tech" alt="html">
                                    </div>
                                    <div class="project--view">
                                        <a href="#">View Project</a>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>
<script>
export default {
    
}
</script>
<style>
    #projects{
        background: #000;
        min-height: 100vh;
        width: 100%;
        position: relative;
    }
    .projects--container{
        min-height: 100vh;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateX(-50%)translateY(-50%);
        width: 100%;
    }
    .projects--container-content{
        margin: 100px 20px;
    }
    .projects--section-header{
        text-align: center;
    }
    .projects--section-header h3{
        color: #fff;
        font-size: 35px;
        text-transform: uppercase;
    }
    .underline-start.light,
    .underline-end.light{
        background: #fff !important;
    }
    .project--container{
        border: 0.1px solid #fff;
        border-radius: 5px;
        color: #fff;
        word-spacing: 5px;
        letter-spacing: 1px;
        margin: 20px 0;
    }
    .project--container .project--header{
        font-size: 20px;
        height: 200px;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .project--container .project--body{
        border-top: 0.1px solid #ffffff;
        padding: 10px;
        text-align: left;
    }
    .project--container .project--footer{
        padding: 10px;
        background: #fff;
        margin: 0 10px 20px 10px;
        display: flex;
    }
    .project--footer-tech{
        width: 20px;
    }
    .project--container .project--view{
        border-top: 0.1px solid #ffffff;
        padding: 10px;
        background: #fff;
        color: #000;
    }
     .project--container .project--view a{
        color: #000;
        text-decoration: none;
    }
</style>