<template>
  <div id="nav">
    <router-link to="/">
      <img src="@/assets/logo.png" alt="" width="50">
    </router-link>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>


<style>
* , ::before, ::after {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    overflow-x: hidden;
}

:root {
    --darkPurple : #18142a;
    --lightPurple: #7264A6;
    --palePink : #F6EBFF;
    --green : #00CEAB;

}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
    width: 100%;
    height: 5rem;
    display: flex;
    background-color: var(--darkPurple);
    place-content: center;
    place-items: center;
}

#nav router-link {
  display: flex;
    place-content: center;
    place-items: center;
    height: 5rem;
    width: 15rem;
    font-size: 1.3rem;
}

</style>
