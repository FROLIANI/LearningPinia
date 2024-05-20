
<template>
  <header>
    <div class="app">
      <nav>
        <RouterLink to="/">Home</RouterLink> | 
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style>
.app{
  text-align: center;

}
</style>


