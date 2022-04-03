<template>
  <div class="vue-tempalte">
    <!-- Navigation -->
    <nav
      class="navbar shadow bg-white rounded justify-content-between flex-nowrap flex-row fixed-top"
    >
      <div class="container">
        <a
          class="navbar-brand float-left"
          target="_blank"
        >
          Student Management
        </a>
        
      </div>
    </nav>

    <!-- Main -->
    <div class="App">
      <div class="vertical-center">
        
          <router-view />
       
      </div>
    </div>
  </div>
</template>
