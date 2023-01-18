<template>
    <h1>{{ courseName }}</h1>
    <p>Course by {{ mentor }}</p>
    <button @click="count++">Count:{{ count }}</button>
</template>
<script>
export default{
    data(){
        return {
            courseName:"Vue Js Learning",
            mentor:"Md Abul Kalam Azad",
            count:0
        }
    }
}

</script>