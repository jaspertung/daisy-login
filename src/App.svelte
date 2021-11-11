<script>
  let username = "";
  let password = "";

  function logIn() {
    return {
      username,
      password,
    };
  }
</script>

<main data-theme="corporate">
  <div class="hero min-h-screen" style="background-image: url(src/assets/presentation-intro-2.png);">
    <div class="hero-overlay bg-opacity-0"></div> 
      <div class="card glass lg:card-side text-neutral-content">
        <div class="max-w-md card-body items-center">
          <h2 class="card-title">Log In</h2>
          <div class="form-control">
            <label for="username" class="label">
              <span class="label-text">Username</span>
            </label>
            <input
              id="username"
              type="text"
              placeholder="username"
              class="input input-bordered lg:w-60"
              bind:value={username}
            />
          </div>

          <div class="form-control">
            <label for="password" class="label">
              <span class="label-text">Password</span>
            </label>
            <input
              id="password"
              type="password"
              placeholder="password"
              class="input input-bordered lg:w-60"
              bind:value={password}
            />
          </div>
          <div class="card-actions">
            <button class="btn btn-primary lg:w-36" on:click={logIn}>Log In</button>
          </div>
          <!-- <p>Logging into {username}'s account</p> -->
        </div>
      </div>
      <!-- if block -->
    </div>
</main>

<style>
  main {
    height: 100vh;
  }
</style>
