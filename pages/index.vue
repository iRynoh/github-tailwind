<template>
  <div class='text-gray-900 text-sm'>
    <TopNav />
    <RepoStats />
    <RepoNav />
    <div class='container mx-auto my-8 px-4 flex'>
      <!--      file-explorer-->
      <div class='container w-3/4 mr-8'>
        <!--        branch-navigation-->
        <div class='flex items-center justify-between'>
          <div class='flex items-center space-x-2'>
            <button class='border border-gray-300 rounded-md px-4 py-1 hover:bg-gray-100  flex items-center space-x-2'>
              <svg class='w-4 fill-current text-gray-500' viewBox='0 0 16 16' aria-hidden='true'>
                <path fill-rule='evenodd'
                      d='M11.75 2.5a.75.75 0 100 1.5.75.75 0 000-1.5zm-2.25.75a2.25 2.25 0 113 2.122V6A2.5 2.5 0 0110 8.5H6a1 1 0 00-1 1v1.128a2.251 2.251 0 11-1.5 0V5.372a2.25 2.25 0 111.5 0v1.836A2.492 2.492 0 016 7h4a1 1 0 001-1v-.628A2.25 2.25 0 019.5 3.25zM4.25 12a.75.75 0 100 1.5.75.75 0 000-1.5zM3.5 3.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0z'></path>
              </svg>
              <span>master</span>
              <svg class='w-3 ml-1' fill='none' stroke='currentColor' viewBox='0 0 24 24'
                   xmlns='http://www.w3.org/2000/svg'>
                <path stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M19 9l-7 7-7-7'></path>
              </svg>
            </button>
            <a href='#' class='flex items-center space-x-1 px-3 py-1 group'>
              <svg class="w-4 fill-current group-hover:text-blue-600" viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M11.75 2.5a.75.75 0 100 1.5.75.75 0 000-1.5zm-2.25.75a2.25 2.25 0 113 2.122V6A2.5 2.5 0 0110 8.5H6a1 1 0 00-1 1v1.128a2.251 2.251 0 11-1.5 0V5.372a2.25 2.25 0 111.5 0v1.836A2.492 2.492 0 016 7h4a1 1 0 001-1v-.628A2.25 2.25 0 019.5 3.25zM4.25 12a.75.75 0 100 1.5.75.75 0 000-1.5zM3.5 3.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0z"></path></svg>
              <div class='group'>
                <span class='font-semibold group-hover:text-blue-600'>31</span>
                <span class='text-gray-500 group-hover:text-blue-600'>branches</span>
              </div>
            </a>
            <a href='#'></a>
          </div>
          <div class='flex items-center space-x-2'>two</div>
        </div>
        <!--        end branch-navigation-->
      </div>
      <!--      end file-explorer-->
      <!--      sidebar-->
      <div class='w-1/4'>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. A, accusantium, aliquid earum enim ipsa laudantium
        magni nulla obcaecati officiis optio perferendis quaerat quas recusandae repellat soluta veniam voluptates!
        Cupiditate, repudiandae.
      </div>
      <!--      end sidebar-->

    </div>
  </div>
</template>
