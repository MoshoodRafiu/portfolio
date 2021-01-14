<template>
    <div>
        <header>
            <vue-particles class="particle--background" color="#dedede"></vue-particles>
            <div class="navigation">
                <div class="navigation--wrapper">
                    <div class="brand--details">
                        <div class="brand--logo-wrapper">
                            <img src="../assets/rom-light.svg" class="brand--logo" alt="logo">
                        </div>
                        <div class="brand--name">ROM</div>
                    </div>
                    <div class="navigation--links" :class="{'toggled': sidebarToggled}">
                        <ul>
                            <li>
                                <a href="#">About</a>
                            </li>
                            <li>
                                <a href="#">Projects</a>
                            </li>
                            <li>
                                <a href="#">Contacts</a>
                            </li>
                            <li>
                                <a href="#" class="cv--download">Download CV</a>
                            </li>
                        </ul>
                    </div>
                    <div class="navigation--toggler" @click="sidebarToggle" :class="{'toggled': sidebarToggled}">
                        <div class="navigation--toggler-line"></div>
                        <div class="navigation--toggler-line"></div>
                        <div class="navigation--toggler-line"></div>
                    </div>
                </div>
            </div>
            <div class="header--container">
                <div class="col-md-7 header--item">
                    <div class="header--item--content">
                        <div class="header--greeting">Hello There!</div>
                        <div class="header--name">I am Rafiu Moshood</div>
                        <div class="header--role">Software Developer</div>
                        <div class="header--socials">
                            <div class="header--social-link"><span class="fab fa-facebook-f"></span></div>
                            <div class="header--social-link"><span class="fab fa-twitter"></span></div>
                            <div class="header--social-link"><span class="fab fa-github"></span></div>
                            <div class="header--social-link"><span class="fab fa-instagram"></span></div>
                            <div class="header--social-link"><span class="fab fa-telegram-plane"></span></div>
                        </div>
                        <div class="header--projects-button-wrapper">
                            <button class="header--projects-button">Projects</button>
                        </div>
                    </div>
                </div>
                <div class="col-md-5 header--item user--image--section">
                    <div class="header--item--content">
                        <img src="../assets/passport.jpg" @mouseover="showBadge" @mouseleave="hideBadge" class="header--user--picture" alt="Rafiu Moshood">
                        <div class="header--user--picture-effect" @mouseover="showBadge" @mouseleave="hideBadge" :style="userImageStyle"></div>
                        <div class="header-badge-detail" :style="{opacity: badgeOpacity}">
                            <span class="fa fa-certificate"></span>
                            <span class="fa fa-ribbon"></span>
                        </div>
                    </div>
                </div>
            </div>
        </header>
    </div>
</template>
<script>
export default {
    name: 'Header',
    data(){
        return{
            imageCoverWidth: 0,
            processing: false,
            badgeOpacity: 0,
            sidebarToggled: false
        }
    },
    created() {
        this.toggleWindowBadge();
    },
    destroyed(){
        clearInterval(this.badgeWindowInterval);
    },
    methods: {
        sidebarToggle(){
            this.sidebarToggled = !this.sidebarToggled;
        },
        toggleWindowBadge(){
            this.badgeWindowInterval = setInterval(() => {
                if (this.imageCoverWidth === 0){
                    this.showBadge();
                }else{
                    this.hideBadge();
                }
            }, 3000)
        },
        showBadge(){
            if (this.imageCoverWidth < 120 && !this.processing){
                 this.processing = true;
                 let showBadgeInteral = setInterval(() => {
                    this.imageCoverWidth += 10;
                    if (this.imageCoverWidth === 120){
                        this.badgeOpacity = 1;
                        this.processing = false;
                        clearInterval(showBadgeInteral);
                    }
                }, 50);
            }
        },
        hideBadge(){
             if (this.imageCoverWidth > 0 && !this.processing){
                 this.badgeOpacity = 0;
                 this.processing = true;
                 let hideBadgeInteral = setInterval(() => {
                    this.imageCoverWidth -= 10;
                    if (this.imageCoverWidth === 0){
                        this.processing = false;
                        clearInterval(hideBadgeInteral);
                    }
                }, 100);
            }
        }
    },
    computed: {
        userImageStyle(){
            return {
                borderRight: `${this.imageCoverWidth}px solid transparent`,
                borderTop: `${this.imageCoverWidth}px solid rgba(0,0,0,0.99)`
            }
        }
    }
}
</script>
<style>
    header{
        width: 100%;
        min-height: 100vh;
        background: black;
        color: white;
    }
    .particle--background{
        position: absolute;
        width: 100%;
        min-height: 100vh;
    }
    .navigation{
        position: absolute;
        width: 100%;
        padding: 40px 100px;
        z-index: 99999;
    }
    .navigation .navigation--wrapper{
        display: flex;
        justify-content: space-between;
    }
    .navigation--toggler{
        padding: 5px;
        display: none;
    }
    .navigation--toggler.toggled 
    .navigation--toggler-line{
        opacity: 0;
    }
    .navigation--toggler.toggled 
    .navigation--toggler-line:first-child,
    .navigation--toggler.toggled 
    .navigation--toggler-line:last-child{
        position: absolute;
        top: 47%;
        opacity: 1;
        transition: 0.4s linear;
    }
    .navigation--toggler.toggled 
    .navigation--toggler-line:first-child{
        transform: rotate(45deg);
    }
    .navigation--toggler.toggled 
    .navigation--toggler-line:last-child{
        transform: rotate(-45deg);
    }
    .navigation--toggler-line{
        height: 3px;
        width: 25px;
        background: #fff;
        margin: 5px 0;
    }
    .navigation .navigation--wrapper .brand--details{
        display: flex;
        align-items: center;
    }
    .navigation .navigation--wrapper .brand--details .brand--logo-wrapper .brand--logo{
        width: 30px;
    }
    .navigation .navigation--wrapper .brand--details .brand--name{
        margin-left: 5px;
        font-size: 25px;
        letter-spacing: 4px;
    }
    .navigation .navigation--wrapper ul li{
        display: inline;
    }
    .navigation .navigation--wrapper ul li a{
        padding: 10px 20px;
        color: #fff;
        text-transform: uppercase;
        font-size: 13px;
        letter-spacing: 3px;
        cursor: pointer;
        text-decoration: none;
    }
    .navigation .navigation--wrapper ul li a.cv--download{
        border: 1px solid #fff;
    }
    .navigation .navigation--wrapper ul li a.cv--download:hover{
        background: #fff;
        color: #000;
        transition: 0.6s linear;
    }
    .header--container{
        display: flex;
        z-index: 9999;
    }
    .header--container 
    .header--item{
        height: 100vh;
        position: relative;
    }
    .header--container 
    .header--item 
    .header--item--content{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateX(-50%)translateY(-50%);
    }
    .header--container 
    .header--item 
    .header--item--content
    .header--greeting{
        font-size: 16px;
        text-transform: uppercase;
        letter-spacing: 4px;
    }
    .header--container 
    .header--item 
    .header--item--content
    .header--name{
        font-size: 70px;
        white-space: nowrap;
        font-weight: bolder;
        text-transform: uppercase;
        letter-spacing: 4px;
        word-spacing: 5px;
    }
    .header--container 
    .header--item 
    .header--item--content
    .header--role{
        font-size: 14px;
        text-transform: uppercase;
        letter-spacing: 2px;
    }
    .header--container 
    .header--item 
    .header--item--content
    .header--socials{
        display: flex;
        margin-top: 15px;
    }
    .header--container 
    .header--item 
    .header--item--content
    .header--socials
    .header--social-link{
        padding: 5px 10px;
        width: 40px;
        text-align: center;
        border: 1px solid #fff;
        border-radius: 5px;
        margin-right: 7px;
        cursor: pointer;
        background: #000;
    }
    .header--container 
    .header--item 
    .header--item--content
    .header--socials
    .header--social-link:hover{
        background: #fff;
        color: #000;
        transition: 0.4s linear;
    }
    .header--container 
    .header--item 
    .header--item--content
    .header--projects-button-wrapper
    .header--projects-button{
        margin-top: 20px;
        padding: 10px 20px;
        width: 230px;
        font-size: 20px;
        text-transform: uppercase;
        border: none;
        background: transparent;
        color: #fff;
        border: 1px solid #ffffff;
        letter-spacing: 3px;
    }
    .header--container 
    .header--item 
    .header--item--content
    .header--projects-button-wrapper
    .header--projects-button:hover{
        background: #fff;
        color: #000;
        transition: 0.4s linear;
    }
    .header--item--content
    .header--user--picture{
        width: 80%;
        border-radius: 0 70px 0 70px;
        border: 5px solid #fff;
    }
    .header--user--picture-effect{
        position: absolute;
        width: 0;
        height: 0;
        top: 0;
        left: 0;
    }
    .header-badge-detail{
        position: absolute;
        top: 25px;
        left: 10px;
        transform: rotate(-45deg);
        letter-spacing: 3px;
        padding: 3px 10px;
        background: #fff;
        color: #000;
        border-radius: 25px;
        cursor: pointer;
        transition: 0.6s linear;
    }
    @media screen and (max-width: 1200px) {
        .header--container 
        .header--item 
        .header--item--content
        .header--name{
            font-size: 50px;
        }
        .header--item--content
        .header--user--picture{
            width: 100%;
        }
    }
    @media screen and (max-width: 800px) {
        .header--container 
        .header--item 
        .header--item--content
        .header--name{
            font-size: 45px;
        }
        .header--item--content
        .header--user--picture{
            width: 100%;
            border-radius: 0 70px 0 70px;
            border: 5px solid #fff;
        }
    }
    @media screen and (max-width: 780px) {
        .header--container 
        .header--item 
        .header--item--content
        .header--name{
            font-size: 45px;
        }
        .header--item.user--image--section{
            display: none;
        }
        .navigation--toggler{
            padding: 5px;
            display: block;
            /* transition: 0.6s linear; */
        }
        .navigation--links ul{
            margin: 0 !important;
            position: absolute;
            background: rgba(0, 0, 0, 0.95);
            left: -100%;
            top: 0;
            width: 60%;
            padding: 50px 20px;
            height: 100vh;
            transition: 0.4s linear;
        }
        .navigation--links.toggled ul{
            left: 0%;
        }
        .navigation--links ul li a{
            display: block;
            margin-bottom: 50px;
        }
    }
     @media screen and (max-width: 500px) {
        .navigation{
            padding: 40px;
        }
        .header--container 
        .header--item 
        .header--item--content
        .header--name{
            font-size: 30px;
        }
    }
    @media screen and (max-width: 350px) {
        .header--container 
        .header--item 
        .header--item--content
        .header--name{
            font-size: 25px;
        }
    }
</style>