<script>
    import Sidebar from './Sidebar.svelte';
    import ChatView from './ChatView.svelte';

    let selectedUser = null;
    let messages = {
        'Alice Johnson': ['Hello!', 'How are you?'],
        'Bob Smith': ['Hi!', 'What\'s up?'],
        // Add more users and their messages here
    };

    function handleUserSelect(user) {
        selectedUser = user;
    }
</script>

<div class="app">
    <div class="fixed top-0 left-[16rem] right-0 shadow z-10 h-[76px] bg-[#24292f] ">
        <div class="flex justify-between items-center p-3">
          <input 
            type="search" 
            placeholder="Search alumni, students or professors" 
            class="search border border-gray-300 focus:border-black focus:outline-none focus:ring-0 transition-all duration-150 ml-2 mt-2 pl-10 rounded-full h-10 w-[60%] bg-no-repeat bg-left bg-center bg-x-[20px] bg-[url('/icon/search.png')] bg-[length:35px]">
          
          <div class="flex gap-3">
            <div class="w-10 h-10 rounded-full flex items-center justify-center hover:bg-[#bfbdbc]">
              <i class="fa-regular fa-bell text-2xl text-white"></i>
            </div>
            <div class="w-10 h-10 rounded-full flex items-center justify-center hover:bg-[#bfbdbc]">
              <img src="/icon/messenger.png" class="max-w-full max-h-full pt-1" alt="">
            </div>
            <div class="w-10 h-10 rounded-full flex items-center justify-center bg-white hover:bg-[#bfbdbc]">
              <i class="fa-solid fa-user"></i>
            </div>
          </div>
        </div>
        </div>
    <Sidebar on:selectUser={e => handleUserSelect(e.detail)} />
    <ChatView user={selectedUser} messages={messages[selectedUser]} />
</div>

<style>
    .app {
        display: flex;
        height: 100vh;
    }
</style>