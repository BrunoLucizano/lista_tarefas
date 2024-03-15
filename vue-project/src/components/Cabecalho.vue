<script setup>
    const props = defineProps(['tarefasPendentes']);
</script>

<template>
    <header class="p-5 mb-4 mt-4 bg-light rounded-3">
        <h1>Minhas Tarefas</h1>
        <p v-if="props.tarefasPendentes === 0">
            Você não tem tarefas pendentes.
        </p>
        <p v-else>
            Você possui {{ props.tarefasPendentes }} tarefa(s) pendente(s).
        </p>
    </header>
</template>