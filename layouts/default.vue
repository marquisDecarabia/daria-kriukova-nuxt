<template>
  <div>
    <nav class="navbar is-danger">
       <div class="navbar-brand">
          <nuxt-link class="navbar-item has-text-centered" to="/">K.D.A. - <span class="icon"><i class="fa fa-bug"></i></span></nuxt-link>
        </div>
      <div class="navbar-menu">
        <div class="navbar-end">
              <nuxt-link class="navbar-item" to="/">Главная</nuxt-link>
              <nuxt-link class="navbar-item" to="/experience">Опыт</nuxt-link>
              <nuxt-link class="navbar-item" to="/blog">Блог</nuxt-link>
          <div class="navbar-item">
            <div class="field is-grouped">
                <p class="control">
                <a class="button is-medium is-light" href="https://github.com/marquisDecarabia">
                  <span class="icon has-text-danger">
                    <i class="fa fa-github"></i>
                  </span>
                 </a>
                </p>
                <p class="control">
                <a class="button is-medium is-light" href="https://vk.com/marquis_decarabia">
                  <span class="icon has-text-danger">
                    <i class="fa fa-vk"></i>
                  </span>
                 </a>
                </p>
            </div>
          </div>
        </div>
      </div>
      </nav>
    <nuxt/>
  </div>
</template>

<style>
/* html
{
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}
*, *:before, *:after
{
  box-sizing: border-box;
  margin: 0;
}
.button--green
{
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}
.button--green:hover
{
  color: #fff;
  background-color: #3b8070;
}
.button--grey
{
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}
.button--grey:hover
{
  color: #fff;
  background-color: #35495e;
} */
</style>
