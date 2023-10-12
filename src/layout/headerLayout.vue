<template>
     <q-header elevated class="bg-light-blue-10 text-white">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="$emit('drawer')" />

        <q-toolbar-title> Productive Crm </q-toolbar-title>
      </q-toolbar>
    </q-header>
</template>

<script>
export default{
    name:"Header"
}
</script>