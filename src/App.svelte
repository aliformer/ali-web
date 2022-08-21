<script>
  let open = false
  const toggle = () => {
    open = !open
  }
</script>

<header class="header "> 
  <button class="menu-button" on:click="{toggle}">
    <svg viewBox="0 0 60 60" width="20" height="20">
      <rect width="100" height="10"></rect>
      <rect y="20" width="100" height="10"></rect>
      <rect y="40" width="100" height="10"></rect>
    </svg>
  </button>
</header>
<div class="wrapper {open === false ? 'nogrid' : ""}"> 
  <nav class="nav {open === true ? 'display': '' }">
    <ul class="nav-list">
      <li><a class="nav-link" href="#">Home</a></li>
      <li><a class="nav-link" href="#">About</a></li>
      <li><a class="nav-link" href="#">Contact</a></li>
    </ul> 
  </nav>
  <main class="main">
  </main>
</div>

