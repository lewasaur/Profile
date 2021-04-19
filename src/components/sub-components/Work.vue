<template>
    <div class="work-exp">
        <div class="work-container">
            <div class="work-left">
                <div class="work-title"> {{ title }} </div>
                <div class="work-company">{{ company }}</div>
                <!-- <div class="description">Description:
                    <div>
                        {{ description }}
                    </div>
                </div> -->
            </div>
            <div class="work-right">
                <div class="work-dates">
                    {{ startDate }}  {{ endDate }}
                </div>
            </div>


        </div>
    </div>
</template>

<script>
export default {
    name: 'Work',
    props: {
        title: {
            type: String
        },
        startDate: {
            type: String
        },
        endDate: {
            type: String
        },
        company: {
            type: String
        },
        description: {
            type: Array
        }
    }
}
</script>

<style scoped>
    .work-exp {
        margin-top: 2%;
    }

    .work-container {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }
    .work-left {
        display: flex;
        flex-direction: column;

    }
    .work-right {
        display: flex;
        flex-direction: column;
        font-size: 0.65em;
    }
    .work-title {
        font-weight: 600;
    }
    .work-company {
        font-weight: 100;
        font-style: italic;
        font-size: 0.7em;
    }

    @media screen and (max-width: 1155px),
    screen and (max-height: 600px) {
        .work-left {
            width: 60%
        }
    }

</style>