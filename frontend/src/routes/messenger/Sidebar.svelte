<script>
  import { createEventDispatcher } from 'svelte';

  const dispatch = createEventDispatcher();

  // Sample user data with names, profile pictures, and statuses
  let users = [
      { name: 'Alice Johnson', image: 'https://randomuser.me/api/portraits/women/1.jpg', status: 'Online' },
      { name: 'Bob Smith', image: 'https://randomuser.me/api/portraits/men/1.jpg', status: 'Offline' },
      { name: 'Charlie Brown', image: 'https://randomuser.me/api/portraits/men/2.jpg', status: 'Busy' },
      { name: 'Diana Prince', image: 'https://randomuser.me/api/portraits/women/2.jpg', status: 'Online' },
      { name: 'Ethan Hunt', image: 'https://randomuser.me/api/portraits/men/3.jpg', status: 'Away' },
      { name: 'Fiona Gallagher', image: 'https://randomuser.me/api/portraits/women/3.jpg', status: 'Online' },
      { name: 'George Washington', image: 'https://randomuser.me/api/portraits/men/4.jpg', status: 'Offline' },
      { name: 'Hannah Montana', image: 'https://randomuser.me/api/portraits/women/4.jpg', status: 'Online' },
      { name: 'Isaac Newton', image: 'https://randomuser.me/api/portraits/men/5.jpg', status: 'Busy' },
      { name: 'Jessica Jones', image: 'https://randomuser.me/api/portraits/women/5.jpg', status: 'Online' },
      { name: 'George Washington', image: 'https://randomuser.me/api/portraits/men/4.jpg', status: 'Offline' },
      { name: 'Hannah Montana', image: 'https://randomuser.me/api/portraits/women/4.jpg', status: 'Online' },
      { name: 'Isaac Newton', image: 'https://randomuser.me/api/portraits/men/5.jpg', status: 'Busy' },
      { name: 'Jessica Jones', image: 'https://randomuser.me/api/portraits/women/5.jpg', status: 'Online' }
  ];

  function handleClick(user) {
      dispatch('selectUser ', user);
  }
</script>

<div class="sidebar ml-20 mt-[76px]">
  <div class="header">
      <h2>Chats</h2>
  </div>
  <div class="user-list hide-scrollbar">
      {#each users as user}
          <div class="user" on:click={() => handleClick(user)}>
              <img src={user.image} alt={user.name} class="profile-pic" />
              <div class="user-info">
                  <div class="user-name">{user.name}</div>
                  <div class="user-status">{user.status}</div>
              </div>
          </div>
      {/each}
  </div>
</div>

<style>
  .sidebar {
      width: 250px;
      background-color: #ffffff;
      border-right: 1px solid #e0e0e0;
      box-shadow: 2px 0 5px rgba(0, 0, 0, 0.1);
      display: flex;
      flex-direction: column;
      font-family: Arial, sans-serif;
  }

  .header {
      padding: 15px;
      background-color: #f5f5f5;
      border-bottom: 1px solid #e0e0e0;
  }

  .header h2 {
      margin: 0;
      font-size: 18px;
      font-weight: bold;
  }

  .user-list {
      overflow-y: auto;
      flex-grow: 1;
  }

  .user {
      display: flex;
      align-items: center;
      padding: 10px 15px;
      cursor: pointer;
      transition: background-color 0.2s;
  }

  .user:hover {
      background-color: #f0f0f0;
  }

  .profile-pic {
      width: 40px;
      height: 40px;
      border-radius: 50%;
      margin-right: 10px;
  }

  .user-info {
      display: flex;
      flex-direction: column;
  }

  .user-name {
      font-weight: bold;
      color: #333;
  }

  .user-status {
      font-size: 12px;
      color: #888;
  }
  .hide-scrollbar::-webkit-scrollbar{
  display: none;
    }
    .hide-scrollbar{
      -ms-overflow-style:none;
      scrollbar-width: none;
    }
</style>