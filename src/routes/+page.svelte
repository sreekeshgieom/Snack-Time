<section class="hero" id="dash">
  <div>
    <p class="eyebrow">Good morning, Chai lovers ☀️</p>
    <h1>Track every sip, every snack, and every smile.</h1>
    <p class="lead">
      Snack Time keeps your team’s morning and evening chai moments organized with gentle reminders,
      friendly summaries, and admin control when someone misses a log.
    </p>
    <div class="hero-actions">
      <button class="primary">Start today’s log</button>
      <button class="ghost">View monthly summary</button>
    </div>
    <div class="quote-card">
      <span>“Chai is a hug in a cup.”</span>
      <span class="author">— Ancient office proverb</span>
    </div>
  </div>
  <div class="hero-visual">
    <div class="steam"></div>
    <div class="steam steam-2"></div>
    <div class="cup">
      <div class="cup-inner"></div>
      <div class="cup-handle"></div>
    </div>
    <div class="vadai">
      <div class="vadai-hole"></div>
    </div>
  </div>
</section>

<section class="grid" id="log">
  <article class="card">
    <header>
      <h2>Morning & Evening Log</h2>
      <p>Twice a day check-in with quick toggles for sugar, milk, and snacks.</p>
    </header>
    <form class="form">
      <div class="input-group">
        <label for="session">Session</label>
        <select id="session">
          <option>Morning</option>
          <option>Evening</option>
        </select>
      </div>
      <div class="input-group">
        <label for="drink">Drink</label>
        <select id="drink">
          <option>Chai</option>
          <option>Coffee</option>
          <option>Milk</option>
        </select>
      </div>
      <div class="input-group">
        <label for="sugar">Sugar</label>
        <div class="pill-group">
          <button type="button">No sugar</button>
          <button type="button" class="active">Little sugar</button>
          <button type="button">Normal</button>
        </div>
      </div>
      <div class="input-group">
        <label for="milk">Milk</label>
        <div class="pill-group">
          <button type="button" class="active">Regular milk</button>
          <button type="button">No milk</button>
          <button type="button">Oat milk</button>
        </div>
      </div>
      <div class="input-group row">
        <label>
          <input type="checkbox" checked /> Took snacks?
        </label>
        <input type="number" min="0" max="6" value="2" />
      </div>
      <div class="input-group">
        <label for="date">Log for date</label>
        <input id="date" type="date" />
        <small>Forgot to log? Backdate an entry in seconds.</small>
      </div>
      <button class="primary" type="button">Save log</button>
    </form>
  </article>
  <article class="card stats" id="insights">
    <header>
      <h2>Monthly Summary</h2>
      <p>See how the team’s energy flows across the month.</p>
    </header>
    <div class="stat-grid">
      <div>
        <h3>42</h3>
        <p>Total chai cups</p>
      </div>
      <div>
        <h3>28</h3>
        <p>Snack count</p>
      </div>
      <div>
        <h3>6</h3>
        <p>Missed logs</p>
      </div>
      <div>
        <h3>4.8★</h3>
        <p>Team mood score</p>
      </div>
    </div>
    <div class="chart">
      <div class="bar" style="--height: 60%">Mon</div>
      <div class="bar" style="--height: 75%">Tue</div>
      <div class="bar" style="--height: 90%">Wed</div>
      <div class="bar" style="--height: 70%">Thu</div>
      <div class="bar" style="--height: 82%">Fri</div>
    </div>
  </article>
</section>

<section class="grid" id="admin">
  <article class="card admin">
    <header>
      <h2>Admin Control Center</h2>
      <p>Mark entries for anyone, edit past days, or remove duplicates.</p>
    </header>
    <div class="admin-actions">
      <div>
        <h4>Quick mark for user</h4>
        <div class="stack">
          <input type="text" placeholder="Search user" />
          <button class="primary" type="button">Mark for user</button>
        </div>
      </div>
      <div>
        <h4>Delete entry</h4>
        <div class="stack">
          <input type="text" placeholder="Entry ID" />
          <button class="ghost" type="button">Remove entry</button>
        </div>
      </div>
    </div>
    <div class="callout">
      <p>✨ Tip: Use the “Missed log” queue to send gentle reminders after evening tea.</p>
    </div>
  </article>
  <article class="card image-card">
    <img
      src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=900&q=80"
      alt="Tea and snacks on a table"
    />
    <div>
      <h3>Chai time moments</h3>
      <p>
        Add fun snack photos, share highlights, and celebrate the day’s most cheerful cup.
      </p>
    </div>
  </article>
</section>

<section class="cta">
  <div>
    <h2>Ready to make chai tracking delightful?</h2>
    <p>Invite your team, set reminders, and let the monthly summary tell the story.</p>
  </div>
  <button class="primary">Create workspace</button>
</section>

<style>
  .hero {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 3rem;
    align-items: center;
    padding: 2rem 0 4rem;
  }

  .eyebrow {
    text-transform: uppercase;
    letter-spacing: 0.2em;
    font-size: 0.8rem;
    color: #a06533;
    font-weight: 600;
  }

  h1 {
    font-size: clamp(2.5rem, 4vw, 3.6rem);
    margin: 0.5rem 0 1rem;
  }

  .lead {
    font-size: 1.1rem;
    color: #5a3a24;
    line-height: 1.6;
  }

  .hero-actions {
    display: flex;
    gap: 1rem;
    margin-top: 1.5rem;
    flex-wrap: wrap;
  }

  .primary {
    background: #ef7b45;
    color: #fff;
    border: none;
    padding: 0.9rem 1.8rem;
    border-radius: 999px;
    font-weight: 600;
    cursor: pointer;
  }

  .ghost {
    background: #fff4dd;
    color: #7b4d2e;
    border: none;
    padding: 0.9rem 1.8rem;
    border-radius: 999px;
    font-weight: 600;
    cursor: pointer;
  }

  .quote-card {
    margin-top: 2rem;
    background: #fffdf7;
    border-radius: 20px;
    padding: 1.2rem 1.5rem;
    box-shadow: 0 12px 30px rgba(139, 94, 60, 0.15);
    display: flex;
    flex-direction: column;
    gap: 0.4rem;
    width: fit-content;
  }

  .author {
    color: #a36b43;
    font-size: 0.9rem;
  }

  .hero-visual {
    position: relative;
    display: grid;
    place-items: center;
    padding: 2rem;
  }

  .cup {
    width: 180px;
    height: 160px;
    background: #f7d8b0;
    border-radius: 0 0 40px 40px;
    position: relative;
    box-shadow: inset 0 -10px 0 #e5b985, 0 18px 40px rgba(139, 94, 60, 0.25);
  }

  .cup-inner {
    position: absolute;
    top: 16px;
    left: 14px;
    right: 14px;
    height: 30px;
    background: #8b5e3c;
    border-radius: 20px;
  }

  .cup-handle {
    position: absolute;
    right: -40px;
    top: 35px;
    width: 60px;
    height: 80px;
    border: 14px solid #f7d8b0;
    border-left: 14px solid transparent;
    border-radius: 50%;
  }

  .steam {
    position: absolute;
    width: 40px;
    height: 120px;
    border-radius: 20px;
    background: linear-gradient(180deg, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    top: -40px;
    animation: float 3s ease-in-out infinite;
  }

  .steam-2 {
    left: 40%;
    animation-delay: 1.2s;
    opacity: 0.7;
  }

  .vadai {
    position: absolute;
    bottom: 10px;
    right: 10px;
    width: 90px;
    height: 90px;
    background: #f0a34a;
    border-radius: 50%;
    box-shadow: inset 0 -10px 0 #d98c3d;
  }

  .vadai-hole {
    position: absolute;
    top: 28px;
    left: 28px;
    width: 34px;
    height: 34px;
    background: #fff4dd;
    border-radius: 50%;
  }

  @keyframes float {
    0%,
    100% {
      transform: translateY(0);
    }
    50% {
      transform: translateY(-12px);
    }
  }

  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
  }

  .card {
    background: #ffffff;
    border-radius: 24px;
    padding: 1.8rem;
    box-shadow: 0 16px 40px rgba(139, 94, 60, 0.1);
    display: flex;
    flex-direction: column;
    gap: 1.2rem;
  }

  .card header h2 {
    margin: 0;
  }

  .form {
    display: grid;
    gap: 1rem;
  }

  .input-group {
    display: grid;
    gap: 0.4rem;
  }

  .input-group.row {
    grid-template-columns: 1fr auto;
    align-items: center;
    gap: 1rem;
  }

  select,
  input[type='number'],
  input[type='date'],
  input[type='text'] {
    padding: 0.6rem 0.9rem;
    border-radius: 12px;
    border: 1px solid #f0dac1;
    font-size: 0.95rem;
  }

  .pill-group {
    display: flex;
    gap: 0.6rem;
    flex-wrap: wrap;
  }

  .pill-group button {
    border: none;
    padding: 0.5rem 0.9rem;
    border-radius: 999px;
    background: #fff4dd;
    cursor: pointer;
  }

  .pill-group .active {
    background: #2d1b0d;
    color: white;
  }

  .stats .stat-grid {
    display: grid;
    grid-template-columns: repeat(2, minmax(120px, 1fr));
    gap: 1rem;
  }

  .stats h3 {
    margin: 0;
    font-size: 2rem;
  }

  .chart {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 0.6rem;
    align-items: end;
    height: 180px;
    margin-top: 0.6rem;
  }

  .bar {
    background: linear-gradient(180deg, #f7b267, #ef7b45);
    height: var(--height);
    border-radius: 12px 12px 4px 4px;
    display: grid;
    place-items: end;
    padding-bottom: 0.5rem;
    color: white;
    font-weight: 600;
  }

  .admin-actions {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1.2rem;
  }

  .stack {
    display: grid;
    gap: 0.6rem;
  }

  .callout {
    background: #fff4dd;
    border-radius: 16px;
    padding: 1rem 1.2rem;
  }

  .image-card {
    overflow: hidden;
    padding: 0;
  }

  .image-card img {
    width: 100%;
    height: 220px;
    object-fit: cover;
  }

  .image-card div {
    padding: 1.5rem;
  }

  .cta {
    margin-top: 3rem;
    background: linear-gradient(120deg, #2d1b0d, #5a3a24);
    color: #fff;
    border-radius: 28px;
    padding: 2rem 3rem;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    gap: 1.5rem;
  }

  @media (max-width: 700px) {
    .hero-actions {
      flex-direction: column;
      align-items: flex-start;
    }

    .input-group.row {
      grid-template-columns: 1fr;
    }

    .cta {
      padding: 2rem;
    }
  }
</style>
