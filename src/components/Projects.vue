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
                                    <div class="project--header" @click="goToSite('https://covisoft.netlify.app')">
                                        <img src="../assets/projects/covisoft.png" alt="">
                                    </div>
                                    <div class="project--body">
                                        A COVID-19 testing web application developed using HTML, CSS, JavaScript, Python, PHP, and MySQL that allows users to take a self-test and then displays a risk level of COVID-19.
                                    </div>
                                    <div class="project--credentials">
                                        <div class="project--credentials-title">
                                            Login Credentials
                                        </div>
                                        <div class="project--credentials-body">
                                            <div class="project--credentials-info">
                                                <div>User:</div>
                                                <div>Not required</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                <div>Admin:</div>
                                                <div>Not required</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                <div>Password:</div>
                                                <div>Not required</div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="project--footer">
                                        <img src="../assets/techs/html.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/css.svg" class="project--footer-tech" alt="css">
                                        <img src="../assets/techs/javascript.svg" class="project--footer-tech" alt="js">
                                        <img src="../assets/techs/jquery.svg" class="project--footer-tech" alt="jquery">
                                        <img src="../assets/techs/php.svg" class="project--footer-tech" alt="php">
                                        <img src="../assets/techs/laravel.svg" class="project--footer-tech" alt="laravel">
                                        <img src="../assets/techs/mysql.svg" class="project--footer-tech" alt="mysql">
                                        <img src="../assets/techs/python.svg" class="project--footer-tech" alt="python">
                                    </div>
                                    <div class="project--view" @click="goToSite('https://covisoft.netlify.app')">
                                        <a href="#">View Project</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-lg-4 col-md-6">
                                <div class="project--container">
                                    <div class="project--header" @click="goToSite('https://devrom-romxchange.herokuapp.com')">
                                        <img src="../assets/projects/romxchange.png" alt="">
                                    </div>
                                    <div class="project--body">
                                        A peer-to-peer cryptocurrency exchange platform developed using HTML, CSS, JavaScript, PHP, and MySQL that allows trading of cryptocurrencies using an escrow service.
                                    </div>
                                    <div class="project--credentials">
                                        <div class="project--credentials-title">
                                            Login Credentials
                                        </div>
                                        <div class="project--credentials-body">
                                            <div class="project--credentials-info">
                                                <div>User:</div>
                                                <div>9jatronics@gmail.com</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Admin:</div>
                                                <div>admin@devrom.tech</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Password:</div>
                                                <div>password</div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="project--footer">
                                        <img src="../assets/techs/html.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/css.svg" class="project--footer-tech" alt="css">
                                        <img src="../assets/techs/javascript.svg" class="project--footer-tech" alt="js">
                                        <img src="../assets/techs/jquery.svg" class="project--footer-tech" alt="jquery">
                                        <img src="../assets/techs/php.svg" class="project--footer-tech" alt="php">
                                        <img src="../assets/techs/laravel.svg" class="project--footer-tech" alt="laravel">
                                        <img src="../assets/techs/mysql.svg" class="project--footer-tech" alt="mysql">
                                    </div>
                                    <div class="project--view" @click="goToSite('https://devrom-romxchange.herokuapp.com')">
                                        <a href="#">View Project</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-lg-4 col-md-6">
                                <div class="project--container">
                                    <div class="project--header" @click="goToSite('https://investapp.netlify.app')">
                                        <img src="../assets/projects/investa.png" alt="">
                                    </div>
                                    <div class="project--body">
                                        A simple investment management website developed using HTML, CSS and JavaScript.
                                    </div>
                                    <div class="project--credentials">
                                        <div class="project--credentials-title">
                                            Login Credentials
                                        </div>
                                           <div class="project--credentials-body">
                                            <div class="project--credentials-info">
                                                <div>User:</div>
                                                <div>Not required</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Admin:</div>
                                                <div>Not required</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Password:</div>
                                                <div>Not required</div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="project--footer">
                                        <img src="../assets/techs/html.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/css.svg" class="project--footer-tech" alt="css">
                                        <img src="../assets/techs/javascript.svg" class="project--footer-tech" alt="js">
                                        <img src="../assets/techs/jquery.svg" class="project--footer-tech" alt="jquery">
                                    </div>
                                    <div class="project--view" @click="goToSite('https://investapp.netlify.app')">
                                        <a href="#">View Project</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-lg-4 col-md-6">
                                <div class="project--container">
                                    <div class="project--header" @click="goToSite('https://etrj.com.ng')">
                                        <img src="../assets/projects/etrj.png" alt="">
                                    </div>
                                    <div class="project--body">
                                        A journal web application developed using HTML, CSS, PHP and MySQL for the faculty of engineering, at Lagos state university.
                                    </div>
                                    <div class="project--credentials">
                                        <div class="project--credentials-title">
                                            Login Credentials
                                        </div>
                                        <div class="project--credentials-body">
                                            <div class="project--credentials-info">
                                                <div>User:</div>
                                                <div>Not Available</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Admin:</div>
                                                <div>Not Available</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Password:</div>
                                                <div>Not Available</div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="project--footer">
                                        <img src="../assets/techs/html.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/css.svg" class="project--footer-tech" alt="css">
                                        <img src="../assets/techs/javascript.svg" class="project--footer-tech" alt="js">
                                        <img src="../assets/techs/jquery.svg" class="project--footer-tech" alt="jquery">
                                        <img src="../assets/techs/php.svg" class="project--footer-tech" alt="php">
                                        <img src="../assets/techs/laravel.svg" class="project--footer-tech" alt="laravel">
                                        <img src="../assets/techs/mysql.svg" class="project--footer-tech" alt="mysql">
                                    </div>
                                    <div class="project--view" @click="goToSite('https://etrj.com.ng')">
                                        <a href="#">View Project</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-lg-4 col-md-6">
                                <div class="project--container">
                                    <div class="project--header" @click="goToSite('https://wordsmith-blog.herokuapp.com')">
                                        <img src="../assets/projects/wordsmith.png" alt="">
                                    </div>
                                    <div class="project--body">
                                        A simple music blog developed using HTML, CSS, JavaScript, NodeJS and MySQL.
                                    </div>
                                    <div class="project--credentials">
                                        <div class="project--credentials-title">
                                            Login Credentials
                                        </div>
                                          <div class="project--credentials-body">
                                            <div class="project--credentials-info">
                                                <div>User:</div>
                                                <div>Not required</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Admin:</div>
                                                <div>Not required</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Password:</div>
                                                <div>Not required</div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="project--footer">
                                        <img src="../assets/techs/html.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/css.svg" class="project--footer-tech" alt="css">
                                        <img src="../assets/techs/javascript.svg" class="project--footer-tech" alt="js">
                                        <img src="../assets/techs/nodejs.svg" class="project--footer-tech" alt="node">
                                        <img src="../assets/techs/mysql.svg" class="project--footer-tech" alt="mysql">
                                    </div>
                                    <div class="project--view" @click="goToSite('https://wordsmith-blog.herokuapp.com')">
                                        <a href="#">View Project</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-lg-4 col-md-6">
                                <div class="project--container">
                                    <div class="project--header" @click="goToSite('https://devrom-gpify.netlify.app')">
                                        <img src="../assets/projects/gpify.png" alt="">
                                    </div>
                                    <div class="project--body">
                                        A GP simulation application developed using HTML, CSS and VueJS for college students
                                    </div>
                                    <div class="project--credentials">
                                        <div class="project--credentials-title">
                                            Login Credentials
                                        </div>
                                        <div class="project--credentials-body">
                                            <div class="project--credentials-info">
                                                <div>User:</div>
                                                <div>Not required</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Admin:</div>
                                                <div>Not required</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Password:</div>
                                                <div>Not required</div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="project--footer">
                                        <img src="../assets/techs/html.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/css.svg" class="project--footer-tech" alt="css">
                                        <img src="../assets/techs/javascript.svg" class="project--footer-tech" alt="js">
                                        <img src="../assets/techs/vue.svg" class="project--footer-tech" alt="vue">
                                    </div>
                                    <div class="project--view" @click="goToSite('https://devrom-gpify.netlify.app')">
                                        <a href="#">View Project</a>
                                    </div>
                                </div>
                            </div>
                            <div class="col-lg-4 col-md-6">
                                <div class="project--container">
                                    <div class="project--header" @click="goToSite('https://devrom-cardgame.netlify.app/')">
                                        <img src="../assets/projects/cardgame.png" alt="">
                                    </div>
                                    <div class="project--body">
                                        A cardgame developed using HTML, CSS and JavaScript.
                                    </div>
                                    <div class="project--credentials">
                                        <div class="project--credentials-title">
                                            Login Credentials
                                        </div>
                                        <div class="project--credentials-body">
                                            <div class="project--credentials-info">
                                                <div>User:</div>
                                                <div>Not required</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Admin:</div>
                                                <div>Not required</div>
                                            </div>
                                            <div class="project--credentials-info">
                                                 <div>Password:</div>
                                                <div>Not required</div>
                                            </div>
                                        </div>
                                    </div>
                                    <div class="project--footer">
                                        <img src="../assets/techs/html.svg" class="project--footer-tech" alt="html">
                                        <img src="../assets/techs/css.svg" class="project--footer-tech" alt="css">
                                        <img src="../assets/techs/javascript.svg" class="project--footer-tech" alt="js">
                                    </div>
                                    <div class="project--view" @click="goToSite('https://devrom-cardgame.netlify.app/')">
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
    name: 'projects',
    methods: {
        goToSite(url){
            window.open(url, '_blank')
        }
    }
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
        border: 0.1px solid #383636;
        border-radius: 5px;
        color: #fff;
        word-spacing: 5px;
        letter-spacing: 1px;
        margin: 40px 0;
        background: #333030;
        /* box-shadow: 0 0 15px #5f5c5c;s */
    }
    .project--container .project--header{
        font-size: 20px;
        border-radius: 5px 5px 0 0;
        display: flex;
        justify-content: center;
        align-items: center;
        overflow: hidden;
    }
    .project--container .project--header img{
        width: 100%;
        border-radius: 10px 10px 0 0;
        transition: 0.6s linear;
        cursor: pointer;
        transform: scale(1.03);
    }
    .project--container .project--header img:hover{
        transform: scale(1.5);
    }
    .project--container .project--body{
        border-top: 0.1px solid #383636;
        padding: 15px 10px;
        text-align: left;
        font-family: 'Noto Sans TC', sans-serif;
        font-size: 13px;
        font-style: 100;
    }
    .project--container .project--credentials{
        padding: 5px 10px;
        background: #fff;
        color: #000;
        margin: 0 10px 20px 10px;
        overflow-x: auto;
        border-radius: 5px;
        font-size: 10px;
        text-align: left;
        font-family: 'Noto Sans TC', sans-serif;
    }
    .project--container .project--credentials .project--credentials-title{
        text-align: center;
        padding-bottom: 3px;
        border-bottom: 0.1px solid #000;
    }
    .project--container
    .project--credentials
    .project--credentials-body{
        padding-top: 3px;
    }
    .project--container
    .project--credentials
    .project--credentials-body
    .project--credentials-info{
        display: flex;
        justify-content: space-between;
        align-items: center;
        overflow-x: auto;
    }
    .project--container .project--footer{
        padding: 10px;
        background: #fff;
        margin: 0 10px 20px 10px;
        display: flex;
        overflow-x: auto;
        border-radius: 5px;
        justify-content: center;
    }
    .project--footer-tech{
        width: 30px;
    }
    .project--container .project--view{
        border-top: 0.1px solid #888585;
        padding: 15px;
        font-family: 'Noto Sans TC', sans-serif;
        font-size: 14px;
        cursor: pointer;
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