<template>
    <div>
        <div>
            <p v-if="listofimages.length">
                {{ "Image " + listofimages[0] }}
            </p>
            
            <p v-if="!listofimages.length">
                no images
            </p>

        </div>

        <div>
            <button @click="cycle">
                s+
            </button>
            <button @click="cycle">
                a
            </button>
            <button @click="cycle">
                b
            </button>
            <button @click="cycle">
                c
            </button>
            <button @click="cycle">
                d
            </button>
            <button @click="cycle">
                e
            </button>
            <button @click="cycle">
                f
            </button>




        </div>




    </div>

</template>

<script>    
import {listofimages, cycle} from "@/components/image.vue"

</script>