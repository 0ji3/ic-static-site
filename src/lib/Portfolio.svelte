<script>
    let projects = [
      { name: 'ETH dApp', url: 'https://d-app-starter-project-six-coral.vercel.app/' },
      { name: 'ETH Yield Farm', url: 'https://yield-farm-starter-project-nine.vercel.app/' },
      { name: 'AVAX Messenger', url: 'https://avax-messenger-eight.vercel.app/' },
    ];
  </script>
  
  <!-- Nav.svelteの`href="#portfolio"`と紐づく`id`を指定する -->
  <section id="portfolio">
    <div class="container mx-auto">
      <div class="py-32">
        <h1 class="text-center mb-10 font-medium text-3xl">PORTFOLIO</h1>
        <div class="flex flex-wrap lg:w-4/5 sm:mx-auto">
          <!-- `each`ブロックでループ処理を行う -->
          {#each projects as project}
            <div class="p-2 md:w-1/3 w-full">
              <div
                class="bg-gray-400 text-white hover:bg-gray-800 cursor-pointer rounded p-4 text-center "
              >
                <a href={project.url}>{project.name}</a>
              </div>
            </div>
          {/each}
        </div>
      </div>
    </div>
  </section>