<template>
    <div id="skills-section">
        <div class="title-container">
            <h1 class="title-page">Skills</h1>
        </div>
        <div class="skills-div">
            <div class="skills-wrapper">
                <div class="skills-technical">
                    <span class="skills-caption">Technical</span>
                    <ul>
                        <li>HTML</li>
                        <li>CSS</li>
                        <li>Javascript Es6</li>
                        <li>VueJS</li>
                        <li>NodeJS</li>
                        <li>Python</li>
                        <li>C++</li>
                        <li>Java</li>
                        <li>MongoDB</li>
                        <li>MySQL</li>
                        <li>Excel</li>
                        <li>Business Analytics</li>
                        <li>Routing and Switching</li>
                    </ul>
                </div>
                <div class="skills-tools">
                    <span class="skills-caption">Tools</span>
                    <ul>
                        <li>VsCode</li>
                        <li>PostMan</li>
                        <li>MongoDB Atlas</li>
                        <li>Packet Tracer</li>
                        <li>Jupyter Notebook</li>
                        <li>MS Office</li>
                        <li>GitHub</li>
                        <li>SourceTree</li>
                        <li>Jira</li>
                    </ul>
                </div>
                <!-- <div class="skills-soft">
                    <span class="skills-caption">Soft</span>
                    <ul>
                        <li>Strong Self-Learning</li>
                        <li>Proactivity</li>
                        <li>Critical Thinking</li>
                        <li>Problem Solving</li>
                    </ul>
                </div> -->
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Skills'
}
</script>

<style scoped>
#skills-section {
    background-color: #9AD0EC;
    min-height: 50vh;
}

.skills-div {
    height: 80%;
    width: 60%;
    margin: auto;
    display: flex;
}

.skills-wrapper {
    display: flex;
    width: 100%;
    flex-direction: row;
    justify-content: space-around;
}

.skills-caption {
    font-size: 2em;
    margin-top: 1.2em;
    justify-content: center;
    align-items: center;
}

ul {
    margin-top: 8%;
}

li {
    list-style: none;
}

@media screen and (max-width: 1155px),
    screen and (max-height: 600px) {
        #skills-section {
            min-height: 60vh;
        }
        .skills-div {
            width: 96%;
        }
        /* .skills-wrapper {
            flex-direction: column;
            justify-content: flex-start;
            align-items: center;
        } */
    }

</style>