<template>
  <footer class="top-footer">
          <div class="footer-bar">
            <div class="flex">
              <h1 class="header-logo">estra inc.</h1>
              <nav class="header-nav">
                <ul>
                  <li><a href="#">home</a></li>
                  <li><a href="#">about</a></li>
                  <li><a href="#">service</a></li>
                  <li><a href="#">works</a></li>
                  <li><a href="#">price</a></li>
                  <li><a href="#">contact</a></li>
                </ul>
              </nav>
            </div>
          </div>
          <small>Copyright 2019 estra inc. All Rights Reserved.</small>
        </footer>
</template>

<style>
.top-footer {
  background: #000;
  text-align: center;
}

.top-footer small {
  text-align: center;
  color: #fff;
}

.footer-bar {
  height: 70px;
  line-height: 70px;
}

.header-logo {
  font-size: 20px;
  font-weight: bold;
  margin-left: 35px;
  color: #fff;
  line-height: 70px;
}

.header-nav li {
  display: inline-block;
  margin-right: 35px;
  font-size: 16px;
}

.header-nav a {
  color: #fff;
}

@media screen and (max-width: 768px) {
  .flex {
    display: none;
  }

  .header-logo {
    margin: 0;
    width: 100%;
    text-align: center;
  }
  
  .header-nav {
    display: none;
  }

  .top-footer {
    margin: 0;
    width: 100%;
    text-align: center;
  }

  .menu-content {
    display: block;
    width: calc(100% - 80px);
    height: 100%;
    text-align: center;
    transition: 0.2s;
    position: fixed;
    top: 0;
    left: calc(-100% - 80px);
    background: #fff;
    color: #333333;
    box-shadow: 80px 0 rgba(38, 98, 213, 0.3);
    z-index: 999;
  }
  .menu-content .menu-title {
    margin: 40px 20px;
    font-size: 2.2rem;
    color: #333333;
    text-align: left;
    font-weight: bold;
  }
  .menu-content li a {
    color: #333333;
    margin: 15px;
    padding: 5px;
    border-bottom: 0.5px solid #2662d5;
    text-decoration: none;
    display: block;
  }
  .menu-content li {
    width: 100%;
    text-align: left;
  }
  .menu-content.open {
    left: 0;
  }
}
</style>