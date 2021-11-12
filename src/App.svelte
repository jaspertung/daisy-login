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
  <div class="hero min-h-screen static" style="background-image: url(src/assets/presentation-intro-2.png);">
      <div class="card text-neutral-content bg-gray-300 bg-opacity-40 absolute right-28">
        <div class="max-w-md card-body items-center">
          <h2 class="card-title text-base-300">Log In</h2>
          <div class="form-control">
            <label for="username" class="label">
              <span class="label-text text-base-300">Username</span>
            </label>
            <input
              id="username"
              type="text"
              placeholder="username"
              class="input input-bordered lg:w-60 text-secondary-focus"
              bind:value={username}
            />
          </div>

          <div class="form-control">
            <label for="password" class="label">
              <span class="label-text text-base-300">Password</span>
            </label>
            <input
              id="password"
              type="password"
              placeholder="password"
              class="input input-bordered lg:w-60 text-secondary-focus"
              bind:value={password}
            />
          </div>
          <div class="card-actions">
            <button class="btn btn-primary lg:w-36 text-base-300" on:click={logIn}>Log In</button>
          </div>
        </div>
      </div>
  </div> 
</main>

<style>
  main {
    height: 100vh;
  }
</style>
