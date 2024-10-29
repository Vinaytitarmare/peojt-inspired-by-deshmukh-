<!-- <script>
    export let user;
  
  
    let messages = [
      { from: user, text: 'Hello!' },
      { from: 'You', text: 'Hi there!' },
    ];
  </script>
  
  <div class="chat">
    <h2>Chat with {user}</h2>
    <div class="messages">
      {#each messages as message}
        <div class="{message.from === 'You' ? 'from-you' : 'from-them'}">
          {message.text}
        </div>
      {/each}
    </div>
  </div>
  
  <style>
    .chat {
      flex-grow: 1;
      padding: 20px;
      background-color: #fff;
    }
    .messages .from-you {
      text-align: right;
    }
    .messages .from-them {
      text-align: left;
    }
  </style> -->
  <script>
    export let user;

    // Placeholder for messages data for each user
    let messages = [
      { from: 'You', text:'hey' },
        { from: user, text: 'heloo' },
        { from: 'You', text:'i got something' },
        { from: user, text: 'what' },
        { from: 'You', text:'blaah blaah' },
        { from: user, text: "Duffer....I won't tolerate any non sense" },
        
        { from: 'You', text:'Sorry' },
        { from: user, text: 'nope' },
        { from: 'You', text:'Maaf kr doo' },
        { from: user, text: 'dance?' },
        { from: 'You', text:"no, i can't" },
        { from: user, text: 'shayarii for ur seniorr??' },
        { from: 'You', text:'Jan ke bhi anjaan bante ho kyu tum, Ek bar nhi do bar dekhke bhi nazarandaazz krti ho kyu tum' },
    ];

    let newMessage = '';

    function sendMessage() {
        if (newMessage.trim()) {
            messages.push({ from: 'You', text: newMessage });
            newMessage = '';
        }
    }
</script>

<div class="chat mt-[110px]">
    <!-- <h2>Chat with {user}</h2> -->
     <div class="fixed h-16 bg-gray-300 w-full top-[76px] left-[330px]  flex justify-start items-center shadow-sm">
     <img src="/icon/prof_person.png" class="size-12 rounded-full mx-2" alt="">
     <p>Godfather</p>
     </div>
   <div class="flex flex-col-reverse overflow-y-hidden mb-8 hide-scrollbar "> <div class="messages hide-scrollbar ">
    {#each messages as message}
        <div class="{message.from === 'You' ? 'from-you' : 'from-them'}">
            {message.text}
        </div>
    {/each}
</div></div>
    <div class="input-container fixed bottom-3 w-[160vh]">
        <input 
            type="text" 
            bind:value={newMessage} 
            placeholder="Type a message..." 
            on:keydown={(e) => e.key === 'Enter' && sendMessage()} 
            class="rounded-2xl"
        />
        <button on:click={sendMessage}>Send</button>
    </div>
</div>

<style>
    .chat {
        flex-grow: 1;
        padding: 20px;
        background-color: #fff;
        border-left: 1px solid #e0e0e0;
        display: flex;
        flex-direction: column;
    }

    .messages {
        flex-grow: 1;
        /* margin: 20px; */
        overflow-y: auto;
        margin-bottom: 10px;
    }

    .from-you {
       
        width:fit-content;
        /* text-align: right; */
        display: flex;
        /* flex-direction: row-reverse; */
        background-color: #e0f7fa;
        padding: 10px;
        border-radius: 5px;
        margin: 20px 0;
        
    }

    .from-them {
        text-align: left;
        width:fit-content;
        background-color: #f1f1f1;
        padding: 10px;
        border-radius: 5px;
        margin: 5px 0;
    }

    .input-container {
        display: flex;
        align-items: center;
    }

    input {
        flex-grow: 1;
        padding: 10px;
        border: 1px solid #ccc;
        border-radius: 25px;
        margin-right: 10px;
    }

    button {
        padding: 10px 15px;
        background-color: #007bff;
        color: white;
        border: none;
        border-radius: 25px;
        cursor: pointer;
    }

    button:hover {
        background-color: #0056b3;
    }
    .hide-scrollbar::-webkit-scrollbar{
  display: none;
    }
    .hide-scrollbar{
      -ms-overflow-style:none;
      scrollbar-width: none;
    }
</style>