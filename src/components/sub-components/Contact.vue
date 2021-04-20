<template>
            <div class=contact-box>
                <div class="contact-content">{{ contactContent }}</div>
                <hr>
                <div class="contact-name"><a :href="contactLink" :target="noLink">{{ contactName }}</a></div>
            </div>

</template>

<script>
export default {
    name: 'Contact',
    props: {
        contactName: {
            type: String
        },
        contactContent: {
            type: String
        },
        contactLink: {
            type: String,
            default: ""
        },
        noLink: {
            type: String,
            default: "_blank"
        }
    }
}
</script>

<style scoped>
.contact-box {
    width: 100%;
    align-items: center;
}

.contact-box + .contact-box {
    margin-top: 4%;
}

.contact-name {
    text-align: center;
}

.contact-box:last-of-type {
    margin-bottom: 2%;
}

.contact-content {
    text-align: center;
}
</style>