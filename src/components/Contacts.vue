<template>
    <div id="contact-section">
        <div class="title-container">
            <h1 class="title-page">Contacts</h1>
        </div>
        <div class="contact-div">
            <Contact 
                contactName="E-Mail"
                contactContent="verwasa.arni@gmail.com"
                contactLink="mailto:verwasa.arni@gmail.com"
            />
            <Contact 
                contactName="Phone"
                contactContent="09XXXXXXXXX"
                contactLink="javascript:void(0);"
                noLink="_self"
            />
            <Contact 
                contactName="LinkedIn"
                contactContent="verwasa-arni"
                contactLink="https://www.linkedin.com/in/verwasa-arni/"
            />
            <Contact 
                contactName="Github"
                contactContent="lewasaur"
                contactLink="https://github.com/lewasaur"
            />
        </div>
    </div>
</template>

<script>
import Contact from './sub-components/Contact'
export default {
    name: 'Contacts',
    components: {
        Contact
    }
}
</script>

<style scoped>
#contact-section {
    background-color: #EFDAD7;
    min-height: 40vh;
}

.contact-div {
    width: 20%;
    margin: auto;
    display: flex;
    flex-direction: column;
}



@media screen and (max-width: 1155px),
    screen and (max-height: 600px){
        .contact-div {
            width: 60%;
        }
    }

</style>