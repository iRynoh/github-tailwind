<template>
  <div class='text-gray-900 text-sm'>
    <TopNav />
    <RepoStats />
    <RepoNav />
    <div class='container mx-auto my-8 px-4 flex'>
      <!-- file-explorer container -->
      <div class='container w-3/4 mr-8 px-2'>
        <!-- branch-navigation-->
        <div class='flex items-center justify-between'>
          <div class='flex items-center space-x-2'>
            <button
              class='border border-gray-300 rounded-md px-4 py-1 bg-gray-50 hover:bg-gray-100 flex items-center space-x-2'>
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
            <a href='#' class='flex items-center space-x-1 px-1 py-1 group'>
              <svg class='w-4 fill-current group-hover:text-blue-600' viewBox='0 0 16 16' aria-hidden='true'>
                <path fill-rule='evenodd'
                      d='M11.75 2.5a.75.75 0 100 1.5.75.75 0 000-1.5zm-2.25.75a2.25 2.25 0 113 2.122V6A2.5 2.5 0 0110 8.5H6a1 1 0 00-1 1v1.128a2.251 2.251 0 11-1.5 0V5.372a2.25 2.25 0 111.5 0v1.836A2.492 2.492 0 016 7h4a1 1 0 001-1v-.628A2.25 2.25 0 019.5 3.25zM4.25 12a.75.75 0 100 1.5.75.75 0 000-1.5zM3.5 3.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0z'></path>
              </svg>
              <div class='group'>
                <span class='font-semibold group-hover:text-blue-600'>31</span>
                <span class='text-gray-500 group-hover:text-blue-600'>branches</span>
              </div>
            </a>
            <a href='#' class='flex items-center space-x-1 px-1 py-1 group'>
              <svg class='w-4 fill-current group-hover:text-blue-600' viewBox='0 0 16 16' aria-hidden='true'>
                <path fill-rule='evenodd'
                      d='M2.5 7.775V2.75a.25.25 0 01.25-.25h5.025a.25.25 0 01.177.073l6.25 6.25a.25.25 0 010 .354l-5.025 5.025a.25.25 0 01-.354 0l-6.25-6.25a.25.25 0 01-.073-.177zm-1.5 0V2.75C1 1.784 1.784 1 2.75 1h5.025c.464 0 .91.184 1.238.513l6.25 6.25a1.75 1.75 0 010 2.474l-5.026 5.026a1.75 1.75 0 01-2.474 0l-6.25-6.25A1.75 1.75 0 011 7.775zM6 5a1 1 0 100 2 1 1 0 000-2z'></path>
              </svg>
              <div class='group'>
                <span class='font-semibold group-hover:text-blue-600'>149</span>
                <span class='text-gray-500 group-hover:text-blue-600'>tags</span>
              </div>
            </a>
          </div>
          <div class='flex items-center space-x-2'>
            <button
              class='border border-gray-300 rounded-md bg-gray-50 hover:bg-gray-100 px-3 py-1.5 flex items-center space-x-2'>
              <span>Go to file</span>
            </button>
            <button
              class='border border-gray-300 rounded-md bg-gray-50 hover:bg-gray-100 px-3 py-1.5 flex items-center space-x-2'>
              <span>Add file</span>
              <svg class='w-3 ml-1' fill='none' stroke='currentColor' viewBox='0 0 24 24'
                   xmlns='http://www.w3.org/2000/svg'>
                <path stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M19 9l-7 7-7-7'></path>
              </svg>
            </button>
            <button
              class='border border-gray-300 rounded-md text-gray-50 bg-green-500 hover:bg-green-600 px-3 py-1.5 flex items-center space-x-2'>
              <svg class='w-4 fill-current text-gray-50' viewBox='0 0 16 16' aria-hidden='true'>
                <path fill-rule='evenodd'
                      d='M7.47 10.78a.75.75 0 001.06 0l3.75-3.75a.75.75 0 00-1.06-1.06L8.75 8.44V1.75a.75.75 0 00-1.5 0v6.69L4.78 5.97a.75.75 0 00-1.06 1.06l3.75 3.75zM3.75 13a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5z'></path>
              </svg>
              <span>Code</span>
              <svg class='w-3 ml-1' fill='none' stroke='currentColor' viewBox='0 0 24 24'
                   xmlns='http://www.w3.org/2000/svg'>
                <path stroke-linecap='round' stroke-linejoin='round' stroke-width='2' d='M19 9l-7 7-7-7'></path>
              </svg>
            </button>
          </div>
        </div>
        <!-- end branch-navigation-->
        <!-- commits container-->
        <div
          class='bg-blue-50 rounded-md rounded-b-none border border-blue-200 border-b-0 flex items-center justify-between px-3 py-3 mt-4'>
          <div class='flex items-center space-x-2'>
            <a href='#' class='mr-1'>
              <img class='rounded-full' src='https://avatars.githubusercontent.com/u/4323180?s=48&amp;v=4' width='24'
                   height='24' alt='@adamwathan'>
            </a>
            <a href='#' class='font-semibold hover:underline'>adamwathan</a>
            <a href='#' class='hover:underline hover:text-blue-600'>Update 1.bug_report.yml</a>
          </div>
          <div class='flex items-end space-x-3'>
            <a href='#'>
              <svg aria-label='0 / 2 checks OK' class='w-4 fill-current text-red-500' viewBox='0 0 16 16' role='img'>
                <path fill-rule='evenodd'
                      d='M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z'></path>
              </svg>
            </a>
            <a href='#' class='font-mono text-xs text-gray-600 hover:underline hover:text-blue-500'>e5c41bb</a>
            <a href='#' class='text-gray-600 hover:underline hover:text-blue-500'>5 days ago</a>
            <a href='#' class='flex items-center space-x-1 group'>
              <svg class='w-4 fill-current group-hover:text-blue-600' viewBox='0 0 16 16' aria-hidden='true'>
                <path fill-rule='evenodd'
                      d='M1.643 3.143L.427 1.927A.25.25 0 000 2.104V5.75c0 .138.112.25.25.25h3.646a.25.25 0 00.177-.427L2.715 4.215a6.5 6.5 0 11-1.18 4.458.75.75 0 10-1.493.154 8.001 8.001 0 101.6-5.684zM7.75 4a.75.75 0 01.75.75v2.992l2.028.812a.75.75 0 01-.557 1.392l-2.5-1A.75.75 0 017 8.25v-3.5A.75.75 0 017.75 4z'></path>
              </svg>
              <div class='group'>
                <span class='font-semibold group-hover:text-blue-600'>3,674</span>
                <span class='text-gray-500 group-hover:text-blue-600'>commits</span>
              </div>
            </a>


          </div>

        </div>
        <!-- end commits container-->
        <!-- file explorer-->
        <div class='rounded-md rounded-t-none border border-gray-200 text-gray-700 divide-y divide-gray-200'>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label='Directory' class='w-4 fill-current text-blue-400' viewBox='0 0 16 16' role='img'>
                <path fill-rule='evenodd'
                      d='M1.75 1A1.75 1.75 0 000 2.75v10.5C0 14.216.784 15 1.75 15h12.5A1.75 1.75 0 0016 13.25v-8.5A1.75 1.75 0 0014.25 3h-6.5a.25.25 0 01-.2-.1l-.9-1.2c-.33-.44-.85-.7-1.4-.7h-3.5z'></path>
              </svg>
              <a href='#' class='hover:underline hover:text-blue-500'>.github</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Update 1.bug_report.yml</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>5 days ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label='Directory' class='w-4 fill-current text-blue-400' viewBox='0 0 16 16' role='img'>
                <path fill-rule='evenodd'
                      d='M1.75 1A1.75 1.75 0 000 2.75v10.5C0 14.216.784 15 1.75 15h12.5A1.75 1.75 0 0016 13.25v-8.5A1.75 1.75 0 0014.25 3h-6.5a.25.25 0 01-.2-.1l-.9-1.2c-.33-.44-.85-.7-1.4-.7h-3.5z'></path>
              </svg>
              <a href='#' class='hover:underline hover:text-blue-500'>__tests__</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Fix invalid arg type </a>
              <a href='#' class='hover:underline text-blue-500'>(#3978)</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>9 days ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label='Directory' class='w-4 fill-current text-blue-400' viewBox='0 0 16 16' role='img'>
                <path fill-rule='evenodd'
                      d='M1.75 1A1.75 1.75 0 000 2.75v10.5C0 14.216.784 15 1.75 15h12.5A1.75 1.75 0 0016 13.25v-8.5A1.75 1.75 0 0014.25 3h-6.5a.25.25 0 01-.2-.1l-.9-1.2c-.33-.44-.85-.7-1.4-.7h-3.5z'></path>
              </svg>
              <a href='#' class='hover:underline hover:text-blue-500'>dist</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Add empty .npmignore so dist files are distributed with releases</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>4 years ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label='Directory' class='w-4 fill-current text-blue-400' viewBox='0 0 16 16' role='img'>
                <path fill-rule='evenodd'
                      d='M1.75 1A1.75 1.75 0 000 2.75v10.5C0 14.216.784 15 1.75 15h12.5A1.75 1.75 0 0016 13.25v-8.5A1.75 1.75 0 0014.25 3h-6.5a.25.25 0 01-.2-.1l-.9-1.2c-.33-.44-.85-.7-1.4-.7h-3.5z'></path>
              </svg>
              <a href='#' class='hover:underline hover:text-blue-500'>jest</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Unify test suites</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>12 days ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label='Directory' class='w-4 fill-current text-blue-400' viewBox='0 0 16 16' role='img'>
                <path fill-rule='evenodd'
                      d='M1.75 1A1.75 1.75 0 000 2.75v10.5C0 14.216.784 15 1.75 15h12.5A1.75 1.75 0 0016 13.25v-8.5A1.75 1.75 0 0014.25 3h-6.5a.25.25 0 01-.2-.1l-.9-1.2c-.33-.44-.85-.7-1.4-.7h-3.5z'></path>
              </svg>
              <a href='#' class='hover:underline hover:text-blue-500'>jit</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Fix invalid arg type </a>
              <a href='#' class='hover:underline text-blue-500'>(#3978)</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>9 days ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label='Directory' class='w-4 fill-current text-blue-400' viewBox='0 0 16 16' role='img'>
                <path fill-rule='evenodd'
                      d='M1.75 1A1.75 1.75 0 000 2.75v10.5C0 14.216.784 15 1.75 15h12.5A1.75 1.75 0 0016 13.25v-8.5A1.75 1.75 0 0014.25 3h-6.5a.25.25 0 01-.2-.1l-.9-1.2c-.33-.44-.85-.7-1.4-.7h-3.5z'></path>
              </svg>
              <a href='#' class='hover:underline hover:text-blue-500'>perf</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Performance improvements + memory leak fix </a>
              <a href='#' class='hover:underline text-blue-500'>(#3032)</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>4 months ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label='Directory' class='w-4 fill-current text-blue-400' viewBox='0 0 16 16' role='img'>
                <path fill-rule='evenodd'
                      d='M1.75 1A1.75 1.75 0 000 2.75v10.5C0 14.216.784 15 1.75 15h12.5A1.75 1.75 0 0016 13.25v-8.5A1.75 1.75 0 0014.25 3h-6.5a.25.25 0 01-.2-.1l-.9-1.2c-.33-.44-.85-.7-1.4-.7h-3.5z'></path>
              </svg>
              <a href='#' class='hover:underline hover:text-blue-500'>scripts</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>make some changes to compat mode</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>5 months ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label='Directory' class='w-4 fill-current text-blue-400' viewBox='0 0 16 16' role='img'>
                <path fill-rule='evenodd'
                      d='M1.75 1A1.75 1.75 0 000 2.75v10.5C0 14.216.784 15 1.75 15h12.5A1.75 1.75 0 0016 13.25v-8.5A1.75 1.75 0 0014.25 3h-6.5a.25.25 0 01-.2-.1l-.9-1.2c-.33-.44-.85-.7-1.4-.7h-3.5z'></path>
              </svg>
              <a href='#' class='hover:underline hover:text-blue-500'>src</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Fix invalid arg type </a>
              <a href='#' class='hover:underline text-blue-500'>(#3978)</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>9 days ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label='Directory' class='w-4 fill-current text-blue-400' viewBox='0 0 16 16' role='img'>
                <path fill-rule='evenodd'
                      d='M1.75 1A1.75 1.75 0 000 2.75v10.5C0 14.216.784 15 1.75 15h12.5A1.75 1.75 0 0016 13.25v-8.5A1.75 1.75 0 0014.25 3h-6.5a.25.25 0 01-.2-.1l-.9-1.2c-.33-.44-.85-.7-1.4-.7h-3.5z'></path>
              </svg>
              <a href='#' class='hover:underline hover:text-blue-500'>stubs</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Add CSS filter support </a>
              <a href='#' class='hover:underline text-blue-500'>(#3923)</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>10 days ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label="File" class='w-4 fill-current text-gray-400' viewBox="0 0 16 16" role="img"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v11.5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25V6H9.75A1.75 1.75 0 018 4.25V1.5H3.75zm5.75.56v2.19c0 .138.112.25.25.25h2.19L9.5 2.06zM2 1.75C2 .784 2.784 0 3.75 0h5.086c.464 0 .909.184 1.237.513l3.414 3.414c.329.328.513.773.513 1.237v8.086A1.75 1.75 0 0112.25 15h-8.5A1.75 1.75 0 012 13.25V1.75z"></path></svg>
              <a href='#' class='hover:underline hover:text-blue-500'>.editorconfig</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Convert new stuff to use ES6 modules</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>4 years ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label="File" class='w-4 fill-current text-gray-400' viewBox="0 0 16 16" role="img"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v11.5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25V6H9.75A1.75 1.75 0 018 4.25V1.5H3.75zm5.75.56v2.19c0 .138.112.25.25.25h2.19L9.5 2.06zM2 1.75C2 .784 2.784 0 3.75 0h5.086c.464 0 .909.184 1.237.513l3.414 3.414c.329.328.513.773.513 1.237v8.086A1.75 1.75 0 0112.25 15h-8.5A1.75 1.75 0 012 13.25V1.75z"></path></svg>
              <a href='#' class='hover:underline hover:text-blue-500'>.eslintignore</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Updated CLI init commend</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>2 years ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label="File" class='w-4 fill-current text-gray-400' viewBox="0 0 16 16" role="img"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v11.5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25V6H9.75A1.75 1.75 0 018 4.25V1.5H3.75zm5.75.56v2.19c0 .138.112.25.25.25h2.19L9.5 2.06zM2 1.75C2 .784 2.784 0 3.75 0h5.086c.464 0 .909.184 1.237.513l3.414 3.414c.329.328.513.773.513 1.237v8.086A1.75 1.75 0 0112.25 15h-8.5A1.75 1.75 0 012 13.25V1.75z"></path></svg>
              <a href='#' class='hover:underline hover:text-blue-500'>.eslintrc.json</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Fix style</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>12 days ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label="File" class='w-4 fill-current text-gray-400' viewBox="0 0 16 16" role="img"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v11.5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25V6H9.75A1.75 1.75 0 018 4.25V1.5H3.75zm5.75.56v2.19c0 .138.112.25.25.25h2.19L9.5 2.06zM2 1.75C2 .784 2.784 0 3.75 0h5.086c.464 0 .909.184 1.237.513l3.414 3.414c.329.328.513.773.513 1.237v8.086A1.75 1.75 0 0112.25 15h-8.5A1.75 1.75 0 012 13.25V1.75z"></path></svg>
              <a href='#' class='hover:underline hover:text-blue-500'>.gitignore</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>swap yarn.lock for package-lock.json</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>12 days ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label="File" class='w-4 fill-current text-gray-400' viewBox="0 0 16 16" role="img"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v11.5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25V6H9.75A1.75 1.75 0 018 4.25V1.5H3.75zm5.75.56v2.19c0 .138.112.25.25.25h2.19L9.5 2.06zM2 1.75C2 .784 2.784 0 3.75 0h5.086c.464 0 .909.184 1.237.513l3.414 3.414c.329.328.513.773.513 1.237v8.086A1.75 1.75 0 0112.25 15h-8.5A1.75 1.75 0 012 13.25V1.75z"></path></svg>
              <a href='#' class='hover:underline hover:text-blue-500'>CHANGELOG.md</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Update changelog</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>10 days ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label="File" class='w-4 fill-current text-gray-400' viewBox="0 0 16 16" role="img"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v11.5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25V6H9.75A1.75 1.75 0 018 4.25V1.5H3.75zm5.75.56v2.19c0 .138.112.25.25.25h2.19L9.5 2.06zM2 1.75C2 .784 2.784 0 3.75 0h5.086c.464 0 .909.184 1.237.513l3.414 3.414c.329.328.513.773.513 1.237v8.086A1.75 1.75 0 0112.25 15h-8.5A1.75 1.75 0 012 13.25V1.75z"></path></svg>
              <a href='#' class='hover:underline hover:text-blue-500'>LICENSE</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Avoid updating license every year</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>3 years ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label="File" class='w-4 fill-current text-gray-400' viewBox="0 0 16 16" role="img"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v11.5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25V6H9.75A1.75 1.75 0 018 4.25V1.5H3.75zm5.75.56v2.19c0 .138.112.25.25.25h2.19L9.5 2.06zM2 1.75C2 .784 2.784 0 3.75 0h5.086c.464 0 .909.184 1.237.513l3.414 3.414c.329.328.513.773.513 1.237v8.086A1.75 1.75 0 0112.25 15h-8.5A1.75 1.75 0 012 13.25V1.75z"></path></svg>
              <a href='#' class='hover:underline hover:text-blue-500'>README.md</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Fix Codecov badge </a>
              <a href='#' class='hover:underline text-blue-500'>(#2678)</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>6 months ago</span>
            </div>
          </div>
          <div class='flex justify-between px-4 py-2 hover:bg-gray-50'>
            <div class='w-4/12 flex items-center space-x-4'>
              <svg aria-label="File" class='w-4 fill-current text-gray-400' viewBox="0 0 16 16" role="img"><path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v11.5c0 .138.112.25.25.25h8.5a.25.25 0 00.25-.25V6H9.75A1.75 1.75 0 018 4.25V1.5H3.75zm5.75.56v2.19c0 .138.112.25.25.25h2.19L9.5 2.06zM2 1.75C2 .784 2.784 0 3.75 0h5.086c.464 0 .909.184 1.237.513l3.414 3.414c.329.328.513.773.513 1.237v8.086A1.75 1.75 0 0112.25 15h-8.5A1.75 1.75 0 012 13.25V1.75z"></path></svg>
              <a href='#' class='hover:underline hover:text-blue-500'>base.css</a>
            </div>
            <div class='w-6/12'>
              <a href='#' class='hover:underline text-gray-500 hover:text-blue-500'>Remove preflight CSS export in favor of base</a>
            </div>
            <div class='w-2/12 text-right'>
              <span class='text-gray-500'>2 years ago</span>
            </div>
          </div>
        </div>
        <!-- end file explorer-->
        <!-- readme container-->
        <div class='rounded-md border border-gray-200 px-4 py-4 mt-4'>
          <h4 class='font-semibold'>README.md</h4>
          <div>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. A deleniti ipsa iure quae quidem reiciendis rerum sed voluptates. Ab adipisci aperiam architecto aspernatur assumenda corporis deserunt dignissimos dolore, doloribus dolorum ea eaque eius eum facilis fugiat harum hic impedit in magnam maxime molestias, mollitia nesciunt nobis nulla odit perferendis porro quidem quis ratione sapiente sequi veniam veritatis voluptatibus! Alias maiores quas totam? Ab architecto assumenda commodi consequatur deserunt distinctio dolor eos et eveniet facilis fugit iste laborum minus necessitatibus nostrum numquam optio pariatur placeat provident quidem quos rerum, veritatis? Amet cupiditate dolor error, iure labore laborum nam obcaecati, omnis perspiciatis quae quos reiciendis, rerum veritatis. Ad alias aperiam, consequatur cum cumque, dolore, doloribus eaque eius enim et excepturi incidunt itaque laborum odio odit optio possimus quaerat quisquam repudiandae vel? Accusantium ad blanditiis dolor dolorem ducimus eius enim error exercitationem expedita ipsa ipsum laborum minus placeat quam, quibusdam sint tempore ut! Ab beatae deserunt dolorem illum quisquam saepe similique ullam? Ab, adipisci aperiam culpa distinctio doloremque dolores dolorum earum eligendi error excepturi fuga ipsa iste itaque iure maxime natus necessitatibus nulla odio pariatur perferendis placeat, praesentium quam quia quis sed sunt tempora voluptatem. Atque eaque exercitationem, expedita magnam magni quo tempora?

          </div>

        </div>
        <!-- end readme container-->
      </div>
      <!-- end file-explorer container -->
      <!-- sidebar-->
      <div class='w-1/4'>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. A, accusantium, aliquid earum enim ipsa laudantium
        magni nulla obcaecati officiis optio perferendis quaerat quas recusandae repellat soluta veniam voluptates!
        Cupiditate, repudiandae.
      </div>
      <!-- end sidebar-->

    </div>
    <!-- footer-->
    <footer class='container mx-auto text-xs border-t border-gray-200 pt-10 pb-14 px-3 flex items-center justify-between'>
      <ul class='flex items-center space-x-12'>
        <li>© 2021 GitHub, Inc.</li>
        <li><a href='#' class='text-blue-500 hover:underline'>Terms</a></li>
        <li><a href='#' class='text-blue-500 hover:underline'>Privacy</a></li>
        <li><a href='#' class='text-blue-500 hover:underline'>Security</a></li>
        <li><a href='#' class='text-blue-500 hover:underline'>Status</a></li>
        <li><a href='#' class='text-blue-500 hover:underline'>Docs</a></li>
      </ul>
      <div>
        <svg class="w-6 fill-current text-gray-300 hover:text-gray-500" viewBox="0 0 16 16" aria-hidden="true"><path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
      </div>
      <ul class='flex items-center space-x-12'>
        <li><a href='#' class='text-blue-500 hover:underline'>Contact Github</a></li>
        <li><a href='#' class='text-blue-500 hover:underline'>Pricing</a></li>
        <li><a href='#' class='text-blue-500 hover:underline'>API</a></li>
        <li><a href='#' class='text-blue-500 hover:underline'>Training</a></li>
        <li><a href='#' class='text-blue-500 hover:underline'>Blog</a></li>
        <li><a href='#' class='text-blue-500 hover:underline'>About</a></li>
      </ul>

    </footer>
    <!-- end footer-->
  </div>
</template>
