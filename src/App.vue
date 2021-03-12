<template>
  <div id="app">
    <header>
      <div id="nav">
        <!-- this is header -->
        <b-navbar
          toggleable="md"
          type="dark"
          variant="dark"
          class="fixed-top text-center"
        >
          <b-navbar-brand href="">
            <router-link to="/"
              ><img
                src="https://scontent.fbkk22-3.fna.fbcdn.net/v/t1.15752-9/s2048x2048/157341365_451540269601832_8715023197152399426_n.png?_nc_cat=103&ccb=1-3&_nc_sid=ae9488&_nc_eui2=AeFkYLA1lxGEYIa7yI_xWwfkr2wrKufpKImvbCsq5-koib1_ymQYqQ932bY_UmCAHNxPu6n8D-Ma1qP_muD05oQG&_nc_ohc=ZX1WHtkB8mQAX9SMUBa&_nc_ht=scontent.fbkk22-3.fna&_nc_tp=30&oh=a3ef9d8a257333bc9ac09bb0146cf952&oe=606FEF81"
                class="d-inline-block align-top"
                height="90"
                width="125"
              />
            </router-link>
          </b-navbar-brand>
          <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
          <b-collapse id="nav-collapse" is-nav>
            <b-navbar-nav>
              <b-nav-item href="#">
                <b-col sm="1">
                  <router-link to="/order"><h3>Order</h3></router-link>
                </b-col></b-nav-item
              >

              <b-nav-item href="#">
                <router-link to="/login"><h3>Login</h3></router-link>
              </b-nav-item>
            </b-navbar-nav>

            <!-- Right aligned nav items -->
          </b-collapse>
        </b-navbar>

        <router-view />
      </div>
    </header>
    <!-- this is footer -->
    <footer>
      <nav class="navbar navbar-light">
        <h2 class="text-dark h2">Contact Me</h2>
      </nav>
    </footer>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 20px;
}

#nav a {
  font-weight: bold;
  color: #ffffff;
}

#nav a.router-link-active {
  color: #f8c10ce7;
}
footer {
  margin-top: 15vh;
  background-image: url("https://office-hero.com/images/product/product_02121_xmWR20_X_400x400.png");
  block-size: 30%;
}
header {
  margin-bottom: 15vh;
  margin-top: 15vh;
}
#b-navbar {
  margin-top: 10vh;
}
</style>
