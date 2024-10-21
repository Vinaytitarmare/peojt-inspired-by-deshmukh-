<script>

	// import '../app.css';	
</script>

<div class="app">
	<!-- navbar//header -->
	<div
	class="h-14  flex flex-row justify-between mt-0 pt-2 pl-2 fixed top-0 left-0 w-full z-10  bg-[#f6fbfe] shadow-b-md"
  >
	<img src="/icon/About.png" alt="" class="mt-1" />
	<div class="flex flex-row justify-around space-x-6 items-center">
	  <div><a href="/web_app/home">Home</a></div>
	  <div><a href="download">Download</a></div>
	  <div><a href="support">Support</a></div>
	  
	  <div><a href="about">About</a></div>
	  <div>
		<button class="bg-[#49b6c5] text-white rounded-2xl mr-3 px-4 py-1"
		  ><a href="login">Login</a></button
		>
	  </div>
	</div>
  </div>
  

	<main>
		<slot />
	</main>

	
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		/* flex: 1;
		
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		margin-top: 56px;
		box-sizing: border-box; */
		margin-top: 60px;

	}


</style>
