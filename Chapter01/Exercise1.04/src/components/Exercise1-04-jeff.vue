<template>
    <div>
        <label>
            Name
            <input 
                type="text" 
                v-model="name"
            />
        </label>
         <label>
            Langague
            <input 
                type="text" 
                v-model="language"
            />
        </label>
        <div>
            <h2>Name: {{ name }}</h2>
            <h2>Language: {{ language }}</h2>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return{
            name: "",
            language: "",
        }
    }
}
</script>