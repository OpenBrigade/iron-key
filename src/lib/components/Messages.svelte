<script>
  let conversation = [
    { message: 'Not leave it in Darkness', id: 1 },
    { message: 'It was said that you would, destroy the Sith, not join them.', id: 2 },
    { message: 'Not leave it in Darkness', id: 1 },
    { message: 'It was said that you would, destroy the Sith, not join them.', id: 2 },
    { message: 'Not leave it in Darkness', id: 1 },
    { message: 'It was said that you would, destroy the Sith, not join them.', id: 2 },
    { message: 'Not leave it in Darkness', id: 1 },
    { message: 'It was said that you would, destroy the Sith, not join them.', id: 2 },
    { message: 'Not leave it in Darkness', id: 1 },
    { message: 'It was said that you would, destroy the Sith, not join them.', id: 2 },
    
  ]
</script>

<div class="flex content-between mr-1 min-h-screen">
  <div class="w-2/12 md:w3/12 border-2 border-gray-800 border-r-cyan-900">
    <ul class="menu bg-base-100 w-56 rounded-box">
        <li><a>Item 1</a></li>
        <li class="bordered"><a>I have border</a></li>
        <li><a>Item 3</a></li>
      </ul>
  </div>

  <div class="mx-2 pl-4 ml-2 mr-4 w-9/12 h-6/6">
    <div class="h-5/6">
      {#each conversation as conv}
        <div class="chat {conv.id === 1 ? 'chat-end' : 'chat-start'}">
          <div class="chat-image avatar">
            <div class="w-10 rounded-full">
              <img src="./static/images/avatar.jpg" />
            </div>
          </div>
          <div class="chat-bubble">{conv.message}</div>
        </div>
      {/each}
    </div>

    <div class="mt-2">
      <div>
        <input type="text" placeholder="Type here" class="input input-bordered input-md w-10/12" />
        <button class="btn gap-2 btn-info ml-1">Send</button>
      </div>
    </div>
  </div>
</div>
