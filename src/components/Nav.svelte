<script>
  export let segment;
</script>

<nav id="navBar">
  <div id="logo">
    <a href="/">
      <img src="logo.jpg" alt="virus logo" />
    </a>
  </div>
  <div id="nav-items">
    <ul>
      <il><a class:is-active={segment === undefined} href="/">Home</a></il>
      <il><a class:is-active={segment === "about"} href="/about">About</a></il>
    </ul>
  </div>
</nav>

<style>
  #navBar {
    display: gird;
    grid-template-columns: 90px 4fr;
    grid-template-rows: 1fr;
    width: 100vw;
    height: 60px;
    display: flex;
    align-items: center;
  }
  img {
    height: 50px;
    width: 90px;
  }
  #nav-items {
    width: 100%;
    margin-left: auto;
  }
  #nav-items a {
    color: black;
  }
  a:hover {
    color: default;
  }
  ul {
    display: flex;
    margin: 0;
    padding: 0;
    justify-content: space-evenly;
    font-size: larger;
  }
  .is-active {
    border-bottom: solid crimson 3px;
  }
  @media (min-width: 769px) {
    nav {
      border-bottom: 1px solid grey;
    }
  }
</style>
