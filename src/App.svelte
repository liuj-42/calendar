<script>
    import Tasks from "./lib/tasks.svelte";
</script>

<main>
  <div id="tasks">
    <Tasks />
  </div>
  <div id="today">
    <h2>Today</h2>
    <div id="today-events">
      <div class="event">
        <h3>Event 1</h3>
        <p>Event 1 description</p>
      </div>
      <div class="event">
        <h3>Event 2</h3>
        <p>Event 2 description</p>
      </div>
      <div class="event">
        <h3>Event 3</h3>
        <p>Event 3 description</p>
      </div>
    </div>
  </div>
  <div id="view">
    <h2>weekly/monthly view here</h2>
  </div>
</main>

<style>
  main {
    display: flex;
    flex-direction: row;
    height: 100%;
  }

  #tasks, #today, #view {
    border: 1px solid fuchsia;
  }
  
  #tasks {
    flex-basis: 20%;
  }
  #today {
    flex-basis: 30%;
  }
  #view {
    flex-basis: 50%;
  }
</style>
