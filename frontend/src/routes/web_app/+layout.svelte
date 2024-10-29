<<<<<<< HEAD

<!-- <script>import Navbar from '/Navbar.svelte'</script> -->
<div class="app">
	<!-- <Navbar /> -->
	<div class="fixed h-screen  bg-[#24292f] text-[#49b6c5] transition-width duration-300 ease-in-out w-64	 " id="sidebar">
       
		<div class="flex items-center p-[6px] pl-3  w-40">
			<div class="flex items-center p-3  ">
				<button id="btn">   <div class=""><i class="fa-solid fa-bars text-6 text-[#49b6c5]   hover:text-[#3093a0] hover:bg-white p-3 rounded-full "></i></div> </button>
				
				<div class=" w-36   ml-1 rounded-md  "><img id="logo_img" src="\icon\About.png" alt="Logo"></div>
			</div>
			</div>
			<div> 
	  
		<div class="options">
		  <ul class="mx-4 my-1">
			<li class="">
			   <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14">
				<a href="home" >
					<i class="fas fa-home mr-3"></i>
					<span class="ml-3 itemm ">Home</span>
				</a>
				<span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900  text-blue-500 py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Home</span>
		   
			   </div> </li>

			   <li class="">
				<div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14">
				 <a href="donate" >
					<i class="fa-solid fa-hand-holding-dollar"></i>
					 <span class="ml-6 itemm ">Donate</span>
				 </a>
				 <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900  text-blue-500 py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Home</span>
			
				</div> </li>

				<li class="">
					<div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14">
					 <a href="project" >
						<i class="fa-solid fa-briefcase"></i>
						 <span class="ml-6 itemm ">Project</span>
					 </a>
					 <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900  text-blue-500 py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Home</span>
				
					</div> </li>
	
					<li> <a href="job" >
						<div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14">
						 
							  <i class="fas fa-user-doctor mr-3"></i>
							  <span class="ml-5 itemm">Jobs</span>
						  
						  <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Job Portal</span>
					 
						</div> </li>
			   <li>
				<a href="alumni" > <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14">      
					<i class="fa-solid fa-user-graduate"></i>
				   <span class="ml-8 itemm">Alumni </span>
			  
			   <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Alumni Directory</span>
		</div>   </a> </li>
			<li><a href="meet" >
			   <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14"> 
				<i class="fa-solid fa-video"></i>
				<span class="ml-7 itemm">Scheduled Meets</span>
		   
			<span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Add Post</span>
	   </div>  </a></li>
			<li>
			  <a href="event" > <div class="flex items-center w-full py-5 pl-4 rounded-md hover:bg-white hover:text-[#3093a0] h-14">  
				<i class="fa-solid fa-calendar-days"></i>
				<span class="ml-7 itemm">Events and Reunions</span>
		  
			<span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Message</span>
	  </div>   </a> </li>
			
			
		</ul>
		</div>
	</div>
	<script>
	  
	
	  let button;
	  let sidebar;
	  let items;
	  let tooltip;
	  let main_part=document.querySelector(".main_part");
	
	  let isCollapsed = false;
	
	  
		button = document.querySelector('#btn');
		sidebar = document.querySelector('#sidebar');
		items = document.querySelectorAll('.itemm');
		tooltip = document.querySelector('.tooltip');
		// let search_logo_space=document.querySelector(".search");
	
		button.onclick = () => {
		  isCollapsed = !isCollapsed;
	
		  sidebar.classList.toggle('w-20');
		  tooltip.classList.toggle('opacity-1');
		  
	
		  if (isCollapsed == false) {
			setTimeout(() => {
			  items.forEach((item) => {
				item.classList.toggle('hidden');
				// main_part.classList.toggle('ml-20');

				// search_logo_space.classList.toggle('ml-36');
			  });
			}, 200);
		  } else {
			items.forEach((item) => {
			  item.classList.toggle('hidden');
			//   main_part.classList.toggle('ml-20');

			 
			});
		  }
		};
	  
	</script>
	  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
	  <style>
		  body {
			font-family: 'Poppins', sans-serif;
		  }
		</style>  
	
	
	</div>
	


	<main class="bg-[#d9d9d9] min-h-screen">
		<slot></slot>
	</main>


<!-- </div> -->

<style>
	.app {
		display: flex;
		flex-direction: row;
		min-height: 100vh;	
		background-color: #d9d9d9;
    /* width:screen-controller; */
    /* overflow: hidden; */
	}

	main {
		flex: 1;
		
		
		width: calc(100% - 72px);
		/* padding: 1rem; */
		width: 100%;
		/* max-width: 64rem; */
		/* margin: 0 auto; */
		/* margin-top: 56px; */
		box-sizing: border-box;
		/* height:3000%; */
		/* margin-top: 60px; */
		/* width: 100%; */
		/* overflow:-moz-hidden-unscrollable; */

		flex-direction: column;
		min-height: 100vh;
	}

	/* main {
		 flex: 1;
		
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		margin-top: 56px;
		box-sizing: border-box; 
		margin-top: 60px; 


	 */
</style>
=======

<!-- <script>import Navbar from '/Navbar.svelte'</script> -->
<div class="app">
	<!-- <Navbar /> -->
	<div class="fixed h-screen  bg-[#24292f] text-[#49b6c5] transition-width duration-300 ease-in-out w-64	 " id="sidebar">
       
		<div class="flex items-center p-[6px] pl-3  w-40">
			<div class="flex items-center p-3  ">
				<button id="btn">   <div class=""><i class="fa-solid fa-bars text-6 text-[#49b6c5]   hover:text-[#3093a0] hover:bg-white p-3 rounded-full "></i></div> </button>
				
				<div class=" w-36   ml-1 rounded-md  "><img id="logo_img" src="\icon\About.png" alt="Logo"></div>
			</div>
			</div>
			<div> 
	  
		<div class="options">
		  <ul class="mx-4 my-1">
			<li class="">
			   <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14">
				<a href="home" >
					<i class="fas fa-home mr-3"></i>
					<span class="ml-3 itemm ">Home</span>
				</a>
				<span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900  text-blue-500 py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Home</span>
		   
			   </div> </li>

			   <li class="">
				<div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14">
				 <a href="donate" >
					<i class="fa-solid fa-hand-holding-dollar"></i>
					 <span class="ml-6 itemm ">Donate</span>
				 </a>
				 <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900  text-blue-500 py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Home</span>
			
				</div> </li>

				<li class="">
					<div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14">
					 <a href="project" >
						<i class="fa-solid fa-briefcase"></i>
						 <span class="ml-6 itemm ">Project</span>
					 </a>
					 <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900  text-blue-500 py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Home</span>
				
					</div> </li>
	
					<li> <a href="job" >
						<div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14">
						 
							  <i class="fas fa-user-doctor mr-3"></i>
							  <span class="ml-5 itemm">Jobs</span>
						  
						  <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Job Portal</span>
					 
						</div> </li>
			   <li>
				<a href="alumni" > <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14">      
					<i class="fa-solid fa-user-graduate"></i>
				   <span class="ml-8 itemm">Alumni </span>
			  
			   <span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Alumni Directory</span>
		</div>   </a> </li>
			<li><a href="meet" >
			   <div class="flex items-center w-full py-5 px-4 rounded-md hover:bg-white  hover:text-[#3093a0] h-14"> 
				<i class="fa-solid fa-video"></i>
				<span class="ml-7 itemm">Scheduled Meets</span>
		   
			<span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Add Post</span>
	   </div>  </a></li>
			<li>
			  <a href="event" > <div class="flex items-center w-full py-5 pl-4 rounded-md hover:bg-white hover:text-[#3093a0] h-14">  
				<i class="fa-solid fa-calendar-days"></i>
				<span class="ml-7 itemm">Events and Reunions</span>
		  
			<span class="tooltip absolute left-full top-1/2 transform -translate-y-1/2 bg-gray-900 text-white py-1 px-2 rounded-md opacity-0 transition duration-300 ease-in-out">Message</span>
	  </div>   </a> </li>
			
			
		</ul>
		</div>
	</div>
	<script>
	  
	
	  let button;
	  let sidebar;
	  let items;
	  let tooltip;
	  let main_part=document.querySelector(".main_part");
	
	  let isCollapsed = false;
	
	  
		button = document.querySelector('#btn');
		sidebar = document.querySelector('#sidebar');
		items = document.querySelectorAll('.itemm');
		tooltip = document.querySelector('.tooltip');
		// let search_logo_space=document.querySelector(".search");
	
		button.onclick = () => {
		  isCollapsed = !isCollapsed;
	
		  sidebar.classList.toggle('w-20');
		  tooltip.classList.toggle('opacity-1');
		  
	
		  if (isCollapsed == false) {
			setTimeout(() => {
			  items.forEach((item) => {
				item.classList.toggle('hidden');
				// main_part.classList.toggle('ml-20');

				// search_logo_space.classList.toggle('ml-36');
			  });
			}, 200);
		  } else {
			items.forEach((item) => {
			  item.classList.toggle('hidden');
			//   main_part.classList.toggle('ml-20');

			 
			});
		  }
		};
	  
	</script>
	  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
	  <style>
		  body {
			font-family: 'Poppins', sans-serif;
		  }
		</style>  
	
	
	</div>
	


	<main class="bg-[#d9d9d9] min-h-screen">
		<slot></slot>
	</main>


<!-- </div> -->

<style>
	.app {
		display: flex;
		flex-direction: row;
		min-height: 100vh;	
		background-color: #d9d9d9;
    /* width:screen-controller; */
    /* overflow: hidden; */
	}

	main {
		flex: 1;
		
		
		width: calc(100% - 72px);
		/* padding: 1rem; */
		width: 100%;
		/* max-width: 64rem; */
		/* margin: 0 auto; */
		/* margin-top: 56px; */
		box-sizing: border-box;
		/* height:3000%; */
		/* margin-top: 60px; */
		/* width: 100%; */
		/* overflow:-moz-hidden-unscrollable; */

		flex-direction: column;
		min-height: 100vh;
	}

	/* main {
		 flex: 1;
		
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		margin-top: 56px;
		box-sizing: border-box; 
		margin-top: 60px; 


	 */
</style>
>>>>>>> 353dd432cf96eb226879df70f665f26ec6f562bc
</div>