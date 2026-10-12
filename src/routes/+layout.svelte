<svelte:head>
  <title>Snack Time | Chai & Vadai Tracker</title>
  <meta
    name="description"
    content="Track chai, coffee, milk, and snacks twice a day with a cheerful dashboard for admins and users."
  />
</svelte:head>

<div class="app-shell">
  <header class="top-bar">
    <div class="brand">
      <div class="logo">☕</div>
      <div>
        <p class="brand-title">Snack Time</p>
        <p class="brand-subtitle">Chai • Coffee • Milk • Vadai</p>
      </div>
    </div>
    <nav class="nav">
      <a href="#dash">Dashboard</a>
      <a href="#log">Log your cup</a>
      <a href="#admin">Admin hub</a>
      <a href="#insights">Insights</a>
    </nav>
    <button class="pill">Log in</button>
  </header>

  <main>
    <slot />
  </main>

  <footer class="footer">
    <div>
      <p class="footer-title">Snack Time Rituals</p>
      <p class="footer-copy">“A cup shared is a story told.”</p>
    </div>
    <div class="footer-links">
      <span>Privacy</span>
      <span>Support</span>
      <span>Team</span>
    </div>
  </footer>
</div>

<style>
  :global(body) {
    margin: 0;
    font-family: 'Plus Jakarta Sans', 'Inter', system-ui, sans-serif;
    background: radial-gradient(circle at top, #fff4dd 0%, #fdf8f1 40%, #f5f5f5 100%);
    color: #2d1b0d;
  }

  :global(a) {
    color: inherit;
    text-decoration: none;
  }

  :global(*) {
    box-sizing: border-box;
  }

  .app-shell {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }

  .top-bar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1.5rem 4rem;
    position: sticky;
    top: 0;
    background: rgba(255, 252, 246, 0.9);
    backdrop-filter: blur(10px);
    z-index: 10;
  }

  .brand {
    display: flex;
    align-items: center;
    gap: 1rem;
  }

  .logo {
    font-size: 1.8rem;
    background: #ffe7bf;
    padding: 0.6rem;
    border-radius: 16px;
    box-shadow: 0 8px 20px rgba(139, 94, 60, 0.15);
  }

  .brand-title {
    margin: 0;
    font-size: 1.1rem;
    font-weight: 700;
  }

  .brand-subtitle {
    margin: 0;
    font-size: 0.9rem;
    color: #8b5e3c;
  }

  .nav {
    display: flex;
    gap: 1.5rem;
    font-weight: 600;
  }

  .nav a {
    padding: 0.35rem 0.6rem;
    border-radius: 999px;
    transition: background 0.2s ease;
  }

  .nav a:hover {
    background: #fff0d2;
  }

  .pill {
    border: none;
    padding: 0.7rem 1.6rem;
    border-radius: 999px;
    background: #2d1b0d;
    color: white;
    font-weight: 600;
    cursor: pointer;
    box-shadow: 0 12px 28px rgba(45, 27, 13, 0.2);
  }

  main {
    flex: 1;
    padding: 2rem 4rem 4rem;
  }

  .footer {
    padding: 2rem 4rem;
    background: #2d1b0d;
    color: #fdf8f1;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .footer-title {
    margin: 0;
    font-size: 1.1rem;
    font-weight: 600;
  }

  .footer-copy {
    margin: 0.4rem 0 0;
    color: #ffe9c7;
  }

  .footer-links {
    display: flex;
    gap: 1.5rem;
    font-size: 0.9rem;
  }

  @media (max-width: 900px) {
    .top-bar {
      flex-direction: column;
      align-items: flex-start;
      gap: 1rem;
      padding: 1.5rem 2rem;
    }

    main {
      padding: 2rem;
    }

    .nav {
      flex-wrap: wrap;
    }

    .footer {
      flex-direction: column;
      align-items: flex-start;
      gap: 1rem;
      padding: 2rem;
    }
  }
</style>
