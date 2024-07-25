<script>
import {ref, onMounted} from 'vue'
import Event from '@/type/Event'
const event = ref<Event>(null)
onMounted(() => {
    // fetch event (by id) and set local event data
})
</script>
<template>
    <div v-if="event">
        <h1>{{  event.title }}</h1>
        <p>{{ event.time }}</p>
        <p>{{ event.description }}</p>
    </div>
</template>