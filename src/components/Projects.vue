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
                            <div class="col-lg-4 col-md-6" v-for="index in 6" :key="index">
                                <div class="project--container">
                                    <div class="project--header">
                                        <img src="../assets/projects/crud.png" alt="">
                                    </div>
                                    <div class="project--body">
                                        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ratione mollitia illum ullam autem eos, tempore illo consequatur aperiam iste nostrum!
                                    </div>
                                    <div class="project--footer">
                                        <img src="../assets/techs/html.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/css.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/javascript.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/vue.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/php.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/laravel.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/mysql.svg" class="project--footer-tech" alt="html">
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
        width: 100%;
        padding: 100px 40px;
        position: relative;
    }
    .projects--container{
        width: 100%;
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
        margin: 40px 0;
    }
    .project--container .project--header{
        font-size: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
        overflow: hidden;
    }
    .project--container .project--header img{
        width: 100%;
        border-radius: 5px 5px 0 0;
        transition: 0.6s linear;
    }
    .project--container .project--header img:hover{
        transform: scale(1.1);
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
        overflow-x: auto;
    }
    .project--footer-tech{
        width: 40px;
    }
    .project--container .project--view{
        border-top: 0.1px solid #ffffff;
        padding: 15px;
        /* background: #fff; */
        /* color: #000; */
    }
     .project--container .project--view a{
        color: #fff;
        text-decoration: none;
        text-transform: uppercase;
    }
    @media screen and (max-width: 500px) {
        #projects{
            padding: 100px 20px;
        }
    }
</style>