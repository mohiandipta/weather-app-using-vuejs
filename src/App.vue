<template>
  <div id="app">
    <main>
      <div class="search_box">
        <input type="text" class="search_bar" placeholder="Search..." />
      </div>

      <div class="wraper_wrap">
        <div class="location_box">
          <div class="location">Northampton, United Kingdom</div>
          <div class="date">Monday</div>
        </div>
      </div>

      <div class="weather_box">
        <div class="temp">9°</div>
        <div class="weather">Rain</div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      API_KEY: "fabaabc13a0dd5ad1732be3ad6125225",
    };
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Titillium+Web:wght@300;400;600;700&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: "Titillium Web", sans-serif;
}

#app {
  background-image: url("./assets/hill.png");
  background-size: cover;
  background-position: bottom;
  transition: 0.6s;
}
main {
  min-height: 100vh;
  padding: 35px;
}
.search_box {
  width: 100%;
  margin-bottom: 30px;
}
.search_box .search_bar {
  display: block;
  width: 100%;
  padding: 15px;
  margin-top: 30px;

  border-radius: 0px 20px 0px 20px;
  border: none;
  background: #202020;
  box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.5);
  outline: none;

  font-family: "Titillium Web", sans-serif;
  font-size: 15px;
  font-weight: 700;
  appearance: none;
  transition: 0.6s;
}
.search_box .search_bar:focus {
  box-shadow: 0px 0px 16px rgba(0, 0, 0, 0.5);
  background-color: rgba(255, 255, 255, 0.75);
  border-radius: 20px 0px 20px 0px;
}

.wraper_wrap {
  padding-top: 30px;
}
.wraper_wrap .location_box .location {
  color: rgba(255, 255, 255, 0.829);
  font-size: 25px;
  font-weight: 800;
  text-align: center;
  text-shadow: 0px 0px 20px rgba(0, 0, 0, 0.5);
}
.wraper_wrap .location_box .date {
  color: rgba(255, 255, 255, 0.8);
  font-size: 20px;
  font-weight: 800;
  text-align: center;
  text-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);
}

.weather_box .temp {
  color: rgba(255, 255, 255, 0.829);
  font-size: 90px;
  font-weight: 800;
  text-align: center;

  margin: 30px 80px;
  background-color: #202020;
  border-radius: 0px 20px 0px 20px;
  box-shadow: 3px 6px 20px rgba(0, 0, 0, 0.5);
}
.weather_box .weather {
  color: rgba(255, 255, 255, 0.875);
  font-size: 40px;
  font-weight: 800;
  text-align: center;
  text-shadow: 0px 0px 20px rgba(0, 0, 0, 0.5);
}
</style>
