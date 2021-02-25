<template>
<div class="space" v-for="task in tasks" :key="task.id">
    <Task :task="task" />
</div>
</template>

<script>
import Task from './Task'
export default {
name: 'Tasks',
components: {
    Task
}, 
props: {
    tasks: Array
}
}
</script>

<style scoped>

.space {
    margin-bottom: 5px;
}
</style>