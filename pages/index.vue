<template>
    <div class="bg-blue-500 text-2xl text-center">
        Hello
        <Button :label="count.value"></Button>
    </div>
</template>

<script setup>
import { Button } from 'primevue';
import { ref } from 'vue';

const count = ref(0);

const onClicked = () => {
    count.value++;
}
</script>