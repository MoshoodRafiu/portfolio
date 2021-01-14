<template>
    <div>
        <section id="projects">
            <div class="projects--container">
                <div class="projects--container-content">
                    <div class="projects--section-header">
                        <h3>Projects</h3>
                        <div class="underline mx-auto">
                            <div class="mx-auto d-flex">
                                <div class="underline-start"></div>
                                <div class="underline-end"></div>
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
        background: #F2EFEF;
        width: 100%;
        padding: 100px 40px;
        position: relative;
        font-family: 'Noto Sans TC', sans-serif;
        color: #7e7d7d;
    }
    .projects--container{
        width: 100%;
    }
    .projects--section-header{
        text-align: center;
    }
    .projects--section-header h3{
        /* color: #000; */
        font-size: 35px;
        text-transform: uppercase;
    }
    .project--container{
        border: 0.1px solid #fff;
        border-radius: 5px;
        /* color: #000; */
        background: #fff;
        word-spacing: 5px;
        letter-spacing: 1px;
        margin: 40px 0;
        box-shadow: 0 0 10px #ccc;
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
        transform: scale(1.2);
    }
    .project--container .project--body{
        border-top: 0.1px solid #000;
        padding: 10px;
        text-align: left;
    }
    .project--container .project--footer{
        padding: 10px;
        background: #F2EFEF;
        border-radius: 5px;
        margin: 0 10px 20px 10px;
        display: flex;
        overflow-x: auto;
    }
    .project--footer-tech{
        width: 40px;
    }
    .project--container .project--view{
        border-top: 0.1px solid #000;
        padding: 15px;
    }
     .project--container .project--view a{
        color: #7e7d7d;
        text-decoration: none;
        text-transform: uppercase;
    }
    @media screen and (max-width: 500px) {
        #projects{
            padding: 100px 20px;
        }
    }
</style>