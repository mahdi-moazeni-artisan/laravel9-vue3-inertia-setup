<template>
      <h1>Home Page!</h1>
      <h2>{{message}}</h2>
      <h2>{{props.title}}</h2>
      <p>
        <button @click="decrement">-</button>
        {{counter}}
        <button @click="increment">+</button>
      </p>
      <hr/>
      <p>
        Linkedin:mahdi-moazeni-artisan
      </p>
      <p>
        Github:mahdi-moazeni-artisan
      </p>
      <p>
        StackOverflow:https://stackoverflow.com/users/21455398/mahdi-moazeni-artisan
      </p>
      <p>
        Email:mahdi.moazeni.artisan@gmail.com
      </p>
      <p>
        Website:https://idea-processors.ir
      </p>
</template>

<script setup>
    import { ref } from 'vue';
    import { defineProps } from 'vue';

    const message="Welcome to my SPA!";
    const counter=ref(0);
    function increment(){
        counter.value++;
    }
    function decrement(){
        counter.value--;
    }
    const props=defineProps(['title']);
</script>

<style>

</style>