<script>
  let username = ""
  let password = ""

  function logIn() {
    return username
    return password
  }
</script>

<main data-theme="corporate">
  <div class="md:container md:max-auto md:space-y-6 bg-white">
    <div class="form-control">
      <!-- svelte-ignore a11y-label-has-associated-control -->
      <label class="label">
        <span class="label-text">Username</span>
      </label> 
      <input type="text" placeholder="username" class="input input-bordered lg:w-60" bind:value={username}>
    </div>

    <div class="form-control">
      <!-- svelte-ignore a11y-label-has-associated-control -->
      <label class="label">
        <span class="label-text">Password</span>
      </label> 
      <input type="text" placeholder="password" class="input input-bordered lg:w-60" bind:value={password}>
    </div>
      
    <button class="btn btn-primary lg:w-60" on:click={logIn}>Log In</button>
    <p>Logging into {username}'s account</p>
  </div>
</main>

<style>

</style>
