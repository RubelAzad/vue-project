<template>
    <h1>{{ course.courseName }}</h1>
    <p>Course by {{ course.mentor }}</p>
    <button @click="count++">+</button>
    <h3>Count:{{ count }}</h3>
    <button @click="count--">-</button>
</template>
//option api
<!-- <script>
export default{
    data(){
        return {
            courseName:"Vue Js Learning",
            mentor:"Md Abul Kalam Azad",
            count:0
        }
    }
}

</script> -->

<!-- <script>
    import { ref } from 'vue';
    export default {
        setup(){
            let count = 0;
            const courseName = "Vue JS Learning";
            const mentor ="Md. Abul Kalam Azad";

        return {
            count, courseName, mentor
        }
    }
   }
</script> -->
//script setup way
<!-- <script setup>
    import { ref } from 'vue';
    let count = ref(0);
    const courseName = ref("Vue JS Learning");
    const mentor =ref("Md. Abul Kalam Azad");
</script> -->

<script setup>
    import { ref, reactive } from 'vue';
    let count = ref(0);
    count.value =10;
    let course = reactive({
        courseName: "Vue JS Learning",
        mentor: "Md. Abul Kalam Azad",
    })

    course.courseName = "abc";
    
</script>