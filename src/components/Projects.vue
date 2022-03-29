<template>
    <div id="projects-section">
        <div class="title-container">
            <h1 class="title-page">Passion Projects</h1>
        </div>
        <div class="projects-div">
        <Project 
            projectId="p1"
            title="JiffyTyper"
            description="A typing game where the user must type out the entire text in the shortest time possible. This webapp has a backend/database where the users can send their own texts. The texts are saved through a database and each text will save the user who has the highest score"
            technologies="EJS, Bootstrap, NodeJs, MongoDB, Express"
            live="https://jiffytyper.herokuapp.com/"
            source="https://github.com/lewasaur/JiffyTyperSource"
            imageLink="jiffyTyperThumb.png"
            imageAlt="Jiffy Typer"
        />
        <Project 
            projectId="p2"
            title="ResinPeace"
            description="A calculator webapp that can help Genshin Impact players keep track on when it's best to login. Genshin Impact is a mobile game where the player can only redeem rewards when they spend resins. Resins can only reach up to 160 and regenerate every 8 minutes."
            technologies="HTML, CSS, Javascript"
            live="https://lewasaur.github.io/resinpeace/"
            source="https://github.com/lewasaur/resinpeace/tree/master"
            imageLink="resinPeaceThumb.png"
            imageAlt="Resin Peace"
        />
        </div>
    </div>
</template>

<script>
import Project from './sub-components/Project'
export default {
    name: 'Skills',
    components: {
        Project
    }
}
</script>

<style scoped>
#projects-section {
    background-color: #FE7F9C;
    min-height: 60vh;
}

.projects-div {
    width: 60%;
    margin: auto;
    display: flex;
    justify-content: space-between;
}


@media screen and (max-width: 1155px),
    screen and (max-height: 600px) {
    .projects-div { 
        flex-direction: column; 
        align-items: center; 
    }
}

</style>