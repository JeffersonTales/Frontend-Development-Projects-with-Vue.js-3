<!-- <template>
    <div>
        <h1>{{ text }}</h1>
    </div>
</template> -->

<template>
    <div>
        <h1 v-once>{{ text }}</h1>
        <h1 v-once v-text="text"></h1>
        <h2 v-html="html"></h2>
        <a
            :href="link.url"
            :target="link.target"
            :tabindex="link.tabindex"
            v-text="link.title"
        >
        </a>
    </div>
</template>


<script setup>
    const text = "Directive text";  
    const html = "Stylise</br>HTML in<br/><b>your data</b>";
    const link = {
        url: "https://google.com",
        target: "_blank",
        tabindex: "0",
        title: "Go to Google",
    };
</script>
