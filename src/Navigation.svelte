<!-- Navigation.svelte -->
<script>
  let title = 'Jiahan Liu';

  const navItems = [
    { label: 'Home', path: '/' },
    { label: 'About', path: '/about' },
  ];
</script>

<nav>
  <div class="title">
    <h1>{title}</h1>
  </div>
  <ul>
    {#each navItems as item}
      <li>
        <a href="{item.path}">{item.label}</a>
      </li>
    {/each}
  </ul>
</nav>

<style>
  nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #fff;
    padding: 1rem;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }

  ul {
    display: flex;
    list-style: none;
    margin: 0;
    padding: 0;
  }

  li {
    margin: 0 1rem;
  }

  a {
    color: #333;
    text-decoration: none;
    font-weight: bold;
    font-size: 1.2rem;
    padding: 0.5rem 1rem;
    border-radius: 4px;
    transition: all 0.3s ease;
  }

  a:hover {
    background-color: #eee;
  }

  .title h1 {
    margin: 0;
    font-size: 1.5rem;
  }

  @media (max-width: 768px) {
    ul {
      flex-direction: column;
    }

    li {
      margin: 0.5rem 0;
    }
  }
</style>
