<template>
    <div id="credentials-section">
        <div class="title-container" >
            <h1 class="title-page">Credentials</h1>
        </div>
        <div class="credentials-div" cl>
            <div class="credential-box"><h2>Work Experience</h2>
                
                <Work
                    title="Software Engineer"
                    company="Hooli Software"
                    startDate="Jun 2021"
                    endDate="- Present"
                />
                <Work 
                    title="Online Course Mentor"
                    company="Adipster Tech Ltd"
                    startDate="Jun 2020"
                    endDate="- Nov 2020"
                />

                <Work 
                    title="Operations Engineer Intern"
                    company="dBC technologies"
                    startDate="Mar 2017"
                    endDate="- Jun 2017"
                />
            </div>
            <div class="credential-box"><h2>Education</h2>
                <Work 
                    title="BS Electronics and Communications Engineering"
                    company="Holy Angel University"
                    startDate="Jun 2013"
                    endDate="- Oct 2018"
                />
            </div>
            <div class="credential-box"><h2>Certifications</h2>
                <Work 
                    title="Licensed Electronics Technician"
                    company="Philippine Regulations Commision"
                    startDate="Apr 2019"
                    endDate=""
                />
                <Work 
                    title="Cisco Certified Entry Networking Technician"
                    company="Cisco Systems"
                    startDate="2019"
                    endDate="- 2022"
                />
            </div>
        </div>
    </div>
</template>

<script>
import Work from './sub-components/Work'
export default {
    name: 'Credentials',
    components: {
        Work
    }
}
</script>

<style scoped>
#credentials-section {
    background-color: #EFDAD7;
    min-height: 80vh;

}

.credentials-div {
    display: flex;
    width: 40%;
    margin: auto;
    height: 80%;
    flex-direction: column;
}

.credential-box {
    /* background-color: green; */
    /* border-style: solid; */
    flex-grow: 0;
}

.credential-box h2 {
    font-size: 1.8em;
    margin: 1em auto;
    text-decoration: underline overline;
}

.credential-box + .credential-box {
    margin-top: 4%;
}

@media screen and (max-width: 1155px),
    screen and (max-height: 600px) {
        .credentials-div {
            width: 96%;
        }
        #credentials-section {
            min-height: 100vh;
        }
    }

</style>