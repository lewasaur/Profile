<template>
    <div id="projects-section">
        <div class="title-container">
            <h1 class="title-page">Passion Projects</h1>
        </div>
        <div class="projects-div">
        <Project 
            projectId="p1"
            title="JiffyTyper"
            description="lorem typing bla bnla bla yes koi no moonlight"
            technologies="EJS, Bootstrap, NodeJs, MongoDB, Express"
            live="https://jiffytyper.herokuapp.com/"
            source="https://github.com/lewasaur/JiffyTyperSource"
            imageLink="jiffyTyperThumb.png"
            imageAlt="Jiffy Typer"
        />
        <Project 
            projectId="p2"
            title="ResinPeace"
            description="lorem resin genshin impact say no koi no moonlight iya iya sen resin 160"
            technologies="HTMl, CSS, Javascript"
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
    background-color: #E64398;
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