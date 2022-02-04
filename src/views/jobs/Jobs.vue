<template>
<h1 >  Jobs </h1>
<div v-for="job in jobs" :key="job.id">
    <router-link :to="{ name: 'JobsDetails', params: { id: job.id }}">
        <h2>{{ job.title }}</h2>
    </router-link>
</div>
</template>

<script>
export default {
data() {
    return{
        jobs:[
    {title: 'Maryah web designer',  id: 1,  details: 'Hello'},
    {title: 'Maryah web developer', id: 2,  details: 'Hello'},
    {title: 'Maryah Vue Developer', id: 3,  details: 'Hello'},

    ]
    }
}
}
</script>

<style>

</style>