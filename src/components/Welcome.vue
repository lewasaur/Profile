<template>
    <div id="welcome-section">
        <div class="welcome-div">
            <div class="picture-section">
                <img src="../assets/avatar.jpg" alt="avatar">
            </div>
            <div class="welcome-text">
                <h1>Hello I'm Arni Verwasa</h1>
                <h2 style="margin-top: 1.5%;">An aspiring software engineer based in Pampanga, Philippines</h2>
                <h4 style="margin-top: 2%;">Thank you for visiting my page. I made this website to showcase my personal projects and abilities as a web developer to attract clients and employers. I also made this to practice my skills on
                    HTML, CSS, Javascript, and VueJS which are the technologies used to make this portfolio website. I'm always open to learning and new opportunities.
                </h4>
            </div>
            
        </div>
    </div>
</template>

<script>
//https://scrimba.com/learn/portfolio/styling-the-titles-and-subtitles-cpDGeWf8
////https://www.youtube.com/watch?v=-Wlt8NRtOpo FLEXBOX CRASH COURSE
export default {
    name: 'Welcome'
}
</script>

<style scoped>
    #welcome-section {
        background-color: #F172A1;
        margin-top: 10vh;
        height: 60vh;


    }
    .welcome-div {
        display: flex;
        width: 60%;
        margin: auto;
        align-items: center;
        justify-content: center;
        height: 100%;
    }
    .picture-section{
        margin-right: 16px;
    }
    .picture-section img {
        width: 254px;
        border-radius: 50%;
        flex: 1 1 20rem;
    }

    .welcome-text {
        flex: 1 1 20rem;
        text-align: center;
    }

    @media screen and (max-width: 1155px),
    screen and (max-height: 600px) {
        #welcome-section {
            min-height: 55vh;
            height: auto;
        }
        .welcome-div {
            width: 96%;
            flex-direction: column;
            margin: auto;
        }
        .picture-section img {
            width: 128px;
            margin: 2em 2em;
        }
        .welcome-text {
            font-size: 1.2em;
        }
        h1 {
            font-size: 1.4em;
        }
    /* @media screen and (max-height: 1155px) {
        #welcome-section {
            height: auto;
            min-height: 55vh;

        }
        .welcome-div {
            width: 96%;
            flex-direction: column;
        }
        .welcome-text {
            margin-bottom: 1rem;
        }
    } */

}
    
</style>