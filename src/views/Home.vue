<script setup lang="ts">
import Timeline from "../components/Timeline.vue"

</script>

<template>
    <Suspense>
    <template #default>
        <Timeline/>
    </template>

    <template #fallback>
        <div>
        <progress class="progress is-primary is-small" max="100"/>
        </div>
    </template>
    </Suspense>
</template>