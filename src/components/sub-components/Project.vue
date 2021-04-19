<template>
    <div class="project-container">
        <!-- <img src="./logo.png" alt="aaaaass" style="width: 128px;"> -->
        <img :src="require(`@/assets/projects/${imageLink}`)" :alt="imageAlt" class="project-img" @click="openModal">
        <h3 class="project-name">{{ title }}</h3>
        <div class="project-modal" :id=" projectId ">
            <div class="project-modal-content">
                <div class="modal-header">
                    <h2 class="project-modal-name">{{ title }}</h2>
                    <span class="close-modal" @click="closeModal">&times;</span>
                </div>
                <div class="modal-body">
                    <div class="project-description">
                        {{ description }}
                    </div>
                    <div class="project-technologies">
                        <b>Technologies used:</b> <span style="font-style: italic">{{ technologies }} </span>
                    </div>
                </div>

                <div class="modal-footer">
                    <a :href="live" target="_blank">Live Demo</a>
                    <a :href="source" target="_blank">Source Code</a>
                </div>

            </div>
        </div>

    </div>
</template>

<script>
export default {
    name: 'Project',
    props: {
        projectId: {
            type: String
        },
        title: {
            type: String
        },
        description: {
            type: String
        },
        technologies: {
            type: String
        },
        live: {
            type: String
        },
        source: {
            type: String
        },
        imageLink: {
            type: String
        },
        imageAlt: {
            type: String
        }
    },

    methods: {
        //https://www.w3schools.com/howto/howto_css_modals.asp
        openModal() {
            // let modal = document.getElementById(this.projectId);
            // modal.style.display = "block";
            document.querySelector("#" + this.projectId).style.display = "block"
        },
        closeModal() {
            // let close = document.getElementByClassName('close-modal')[0];
            // close.onclick = function() {
            //     modal.style.display = 'none';
            // }
            document.querySelector("#" + this.projectId).style.display = 'none';
        }
    }
}
</script>

<style scoped>
    .project-container {
        width: 32%;
        padding-bottom: 32%;
        margin-bottom: 2%;
    }


    .project-modal {
        display: none; /* Hidden by default */
        position: fixed; /* Stay in place */
        z-index: 1; /* Sit on top */
        padding-top: 100px; /* Location of the box */
        left: 0;
        top: 0;
        width: 100%; /* Full width */
        height: 100%; /* Full height */
        overflow: auto; /* Enable scroll if needed */
        background-color: rgb(0,0,0); /* Fallback color */
        background-color: rgba(0,0,0,0.4); /* Black w/ opacity */
    }

    .project-modal-content {
        position: relative;
        background-color: #fefefe;
        margin: auto;
        padding: 0;
        border: 1px solid #888;
        width: 80%;
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2),0 6px 20px 0 rgba(0,0,0,0.19);
    }

    .modal-header {
        padding: 2px 16px;
        background-color: #F172A1;
        color: white;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .modal-body {
        padding: 2px 16px;
        background-color: #B39BC8;
        }

    .modal-footer {
        padding: 2px 16px;
        background-color: #F172A1;
        color: white;
    }

    .close-modal {
    font-size: 28px;
    font-weight: bold;
    }

    .close-modal:hover, .close-modal:focus {
    color: black;
    text-decoration: none;
    cursor: pointer;
    }

    .project-img {
        cursor: pointer;
        width: 100%;
        height: 90%;
        border: #800080 solid 3px;
    }

    .project-name {
        text-align: center;
        width: 100%;
    }

    .modal-footer a {
        margin-right: 4%;
    }

    @media screen and (max-width: 1155px),
    screen and (max-height: 600px) {
        .project-container {
            width: 100%;
        }
        .project-modal-name {
            font-size: 1.2em;
            margin-top: 1.6%;
        }
    }

</style>