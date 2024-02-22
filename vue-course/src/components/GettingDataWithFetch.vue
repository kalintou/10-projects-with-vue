<script setup>
import {ref} from 'vue'
const data = ref(null)

const fetchData = () => {
    //Make Make a GET request using fetch
    fetch('https://jsonplaceholder.typicode.com/todos/1').then((response) => {
        //Check if the response status is OK
        if(!response.ok) {
            throw new Error('HTTP Error! Status: ${response.status}')
        }
        //Parse the JSON response
        return response.json()
    }).then((responseData) => {
        data.value = responseData
    }).catch((error) => {
        console.error(`Error fetcing data: ${error}`)
    })
}
</script>

<template>
    <div>
        <h1>(( Using Fetch ))</h1>
        <button @click="fetchData">FetchData</button>
        <div>
            <h2>Data from API:</h2>
            <pre>{{ data }}</pre>
        </div>
    </div>
</template>