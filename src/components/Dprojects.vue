<template>
    <div id="dprojects-section">
        <div class="title-container">
            <h1 class="title-page">Data Projects</h1>
        </div>
        <div class="dprojects-div">
        <Project 
            projectId="p3"
            title="Songs Data Analysis"
            description="An analysis made on my Distrokid(Music Distributing Platform) Data using Python to see which of my songs are doing well and which platforms and countries have big sales. "
            technologies="Python, Pandas, Matplotlib"
            live="https://github.com/lewasaur/Song_Sales_Analysis/blob/main/Distrokid%20Data.ipynb"
            source="https://github.com/lewasaur/Song_Sales_Analysis"
            imageLink="stock_data.jpeg"
            imageAlt="Data Analyst Project"
        />
        <Project 
            projectId="p4"
            title="Chinook Music StoreDB Analysis"
            description="My personal analysis for the Chinook Music Store Database "
            technologies="Python, Pandas, Seaborn, SQL"
            live="https://github.com/lewasaur/Chinook_DB_Analysis/blob/master/Chinook%20Music%20Store%20DB%20analysis.ipynb"
            source="https://github.com/lewasaur/Chinook_DB_Analysis"
            imageLink="stock_data.jpeg"
            imageAlt="Data Analyst Project"
        />
        </div>
    </div>
</template>

<script>
import Project from './sub-components/Project'
export default {
    name: 'Dprojects',
    components: {
        Project
    }
}
</script>

<style scoped>
#dprojects-section {
    background-color:#9AD0EC;
    min-height: 60vh;
}

.dprojects-div {
    width: 60%;
    margin: auto;
    display: flex;
    justify-content: space-between;
}


@media screen and (max-width: 1155px),
    screen and (max-height: 600px) {
    .dprojects-div { 
        flex-direction: column; 
        align-items: center; 
    }
}

</style>