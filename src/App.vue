<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style>
* {
  box-sizing: border-box;
}

body {
  padding: 20px;
  background-color: #0f0f0f;
  color: #f0f0f0;
  font-family: "Cabin", sans-serif;
  font-size: 18px;
}

a {
  color: inherit;
}

img {
  max-width: 100%;
}

.series-listing {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.series-card {
  margin: 20px;
  max-width: 210px;
  overflow: hidden;
  background-color: #f0f0f0;
  color: #0f0f0f;
  border-radius: 20px;
  transition: transform 0.2s;
}

.series-card:hover {
  transform: scale(1.05);
}

.series-card-link {
  text-decoration: none;
}

.series-card-poster {
  display: block;
}

.series-card-header {
  padding: 20px;
}

.series-card-title {
  margin-top: 0;
  font-size: 24px;
  font-weight: 700;
}

.series-genres {
  margin-bottom: 0;
  padding: 0;
  list-style: none;
}

.series-genres-label {
  display: inline;
}

.series-genres-item {
  margin: 0;
  display: inline;
}

.series-genres-item:not(:last-child)::after {
  content: ", ";
}

.series-details {
  max-width: 960px;
  margin: 0 auto;
  padding: 20px;
  background-color: #f0f0f0;
  color: #0f0f0f;
  border-radius: 20px;
}

.is-favorite {
  box-shadow: 0 0 10px red;
}

.series-details-poster {
  display: block;
  margin: 0 auto;
  border-radius: 20px;
}

.series-details-title {
  font-size: 30px;
}

@media screen and (min-width: 600px) {
  .series-details {
    display: flex;
    align-items: flex-start;
  }

  .series-details-poster {
    margin-right: 20px;
  }

  .series-details-body {
    flex: 1;
  }

  .series-details-title {
    margin-top: 0;
  }
}
</style>
