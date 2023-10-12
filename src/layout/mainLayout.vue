<template>
    <div class="q-pa-md">
      <q-layout view="lHh Lpr lff">
        <q-header elevated class="bg-cyan-8">
          <q-toolbar>
            <q-toolbar-title>Dashboard</q-toolbar-title>
            <q-btn flat @click="drawer = !drawer" round dense icon="menu" />
          </q-toolbar>
        </q-header>
  
        <q-drawer
          v-model="drawer"
          :mini="!drawer || miniState"
          show-if-above
          :width="200"
          :breakpoint="400"
        >
          
  
        
        </q-drawer>
  
        <q-page-container>
          <q-page>
           <router-view/>
          </q-page>
        </q-page-container>
      </q-layout>
    </div>
  </template>
  
  <script>
  import { ref } from 'vue'
  
  export default {
    setup () {
      return {
        drawer: ref(false)
      }
    }
  }
  </script>
  