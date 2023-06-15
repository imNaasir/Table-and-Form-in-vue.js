<template>
    <div class="container mx-auto px-20 py-10">
        <div class=" w-full h-auto my-4 mx-auto ">
            <div class="bg-white w-full rounded-md py-5 flex flex-col gap-3  lg:flex-row px-4 justify-between items-center">
                <div class="flex flex-row items-center gap-2">
                    <span class="font-[ui-sans-serif - 700] text-[22px] font-[700] text-black ">Get your data</span>
                </div>
                <div class="text-center 
                bg-[#BD3401] py-1 px-2 rounded-md text-black ">
                <button class="text-xl font-[500] text-white" @click="updatePage">New Record</button>
                </div>
            </div>
        </div>
        <table class="border border-collapse w-full bg-white px-8">
                <thead class="">
                    <tr class="">
                        <td class="flex items-center justify-center bg-white py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 invisible"></td>
                        <th class="bg-white py-2 "></th>
                        <th class="text-left bg-white py-3 text-xl font-bold">Name</th>
                        <th class="text-left bg-white py-3 text-xl font-bold">Compony</th>
                        <th class="text-left bg-white py-3 text-xl font-bold">City</th>
                        <th class="text-left bg-white py-3 text-xl font-bold">Progress</th>
                        <th class="text-left bg-white py-3 text-xl font-bold">Created</th>
                        <th class="text-left bg-white py-3 text-xl font-bold"></th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="">
                        <td class="flex items-center justify-center py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 "></td>
                        <td class="py-2">
                            <div class="image ">
                                <img src="https://avatars.dicebear.com/v2/initials/john-doe.svg" alt="" class="w-6 h-6 rounded-full
                                    ml-auto mr-auto block">
                            </div>
                        </td>
                        <td class=" text-left py-2">Rebecca Bauch</td>
                        <td class=" text-left py-2">Daugherty-Daniel</td>
                        <td class=" text-left py-2">South Cory</td>
                        <td class=" text-left py-2">
                            <div class="bg-[#E5E7EB] w-24 h-3 rounded-xl">
                                <div class="row1 bg-blue-500 w-20 h-3 rounded-xl" ></div>
                            </div>
                        </td>
                        <td class=" text-left py-2">Oct 25, 2021</td>
                        <td class=" text-left py-2">
                            <div class="flex items-center gap-1 text-white justify-center">
                                <button class="bg-[#3B82F6] hover:bg-[#2563EB] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    
                                </button>
                                <button class="bg-red-500 hover:bg-[#DC2626] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                                    </svg>
                                    
                                </button>
                            </div>
                        </td>
                    </tr>
                    <tr class="">
                        <td class="flex items-center justify-center py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 "></td>
                        <td class="py-2">
                            <div class="image ">
                                <img src="https://avatars.dicebear.com/v2/initials/felicita-yundt.svg" class="rounded-full
                                ml-auto mr-auto block w-6 h-6">
                            </div>
                        </td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">
                            <div class="bg-[#E5E7EB] w-24 h-3 rounded-xl">
                                <div class="row2 bg-blue-500 w-16 h-3 rounded-xl" ></div>
                            </div>
                        </td>
                        <td class=" text-left py-2">Jan 8, 2021</td>
                        <td class=" text-left py-2">
                            <div class="flex items-center gap-1 text-white justify-center">
                                <button class=" bg-[#3B82F6] hover:bg-[#2563EB] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    
                                </button>
                                <button class="bg-red-500 hover:bg-[#DC2626] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                                    </svg>
                                    
                                </button>
                            </div>
                        </td>
                    </tr>
                    <tr class="">
                        <td class="flex items-center justify-center py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 "></td>
                        <td class="py-2">
                            <div class="image ">
                                <img src="https://avatars.dicebear.com/v2/initials/mr-larry-satterfield-v.svg" class="rounded-full
                                w-6 h-6 ml-auto mr-auto">
                            </div>
                        </td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">
                            <div class="bg-[#E5E7EB] w-24 h-3 rounded-xl">
                                <div class="row3 bg-blue-500 w-4 h-3 rounded-xl" ></div>
                            </div>
                        </td>
                        <td class=" text-left py-2">Jan 8, 2021</td>
                        <td class=" text-left py-2">
                            <div class="flex items-center gap-1 text-white justify-center">
                                <button class="bg-[#3B82F6] hover:bg-[#2563EB] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    
                                </button>
                                <button class="bg-red-500 hover:bg-[#DC2626] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                                    </svg>
                                    
                                </button>
                            </div>
                        </td>
                    </tr>
                    <tr class="">
                        <td class="flex items-center justify-center py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 "></td>
                        <td class="py-2">
                            <div class="image ">
                                <img src="https://avatars.dicebear.com/v2/initials/mr-broderick-kub.svg"  alt="" class="w-6 h-6 rounded-full
                                    ml-auto mr-auto block">
                            </div>
                        </td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">
                            <div class="bg-[#E5E7EB] w-24 h-3 rounded-xl">
                                <div class="row4 bg-blue-500 w-10 h-3 rounded-xl" ></div>
                            </div>
                        </td>
                        <td class=" text-left py-2">Jan 8, 2021</td>
                        <td class=" text-left py-2">
                            <div class="flex items-center gap-1 text-white justify-center">
                                <button class="bg-[#3B82F6] hover:bg-[#2563EB] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    
                                </button>
                                <button class="bg-red-500 hover:bg-[#DC2626] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                                    </svg>
                                    
                                </button>
                            </div>
                        </td>
                    </tr>
                    
                    <tr class="">
                        <td class="flex items-center justify-center py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 "></td>
                        <td class="py-2">
                            <div class="image ">
                                <img src="https://avatars.dicebear.com/v2/initials/barry-weber.svg" alt="" class="w-6 h-6 rounded-full
                                    ml-auto mr-auto block">
                            </div>
                        </td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">
                            <div class="bg-[#E5E7EB] w-24 h-3 rounded-xl">
                                <div class="row5 bg-blue-500 w-[2.5rem] h-3 rounded-xl" ></div>
                            </div>
                        </td>
                        <td class=" text-left py-2">Jan 8, 2021</td>
                        <td class=" text-left py-2">
                            <div class="flex items-center gap-1 text-white justify-center">
                                <button class="bg-[#3B82F6] hover:bg-[#2563EB] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    
                                </button>
                                <button class="bg-red-500 hover:bg-[#DC2626] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                                    </svg>
                                    
                                </button>
                            </div>
                        </td>
                    </tr>
                    <tr class="">
                        <td class="flex items-center justify-center py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 "></td>
                        <td class="py-2">
                            <div class="image ">
                                <img src="https://avatars.dicebear.com/v2/initials/bert-kautzer-md.svg" alt="" class="w-6 h-6 rounded-full
                                    ml-auto mr-auto block">
                            </div>
                        </td>
                        <td class=" text-left py-2">Rebecca Bauch</td>
                        <td class=" text-left py-2">Daugherty-Daniel</td>
                        <td class=" text-left py-2">South Cory</td>
                        <td class=" text-left py-2">
                            <div class="bg-[#E5E7EB] w-24 h-3 rounded-xl">
                                <div class="row6 bg-blue-500 w-[3.8rem] h-3 rounded-xl" ></div>
                            </div>
                        </td>
                        <td class=" text-left py-2">Oct 25, 2021</td>
                        <td class=" text-left py-2">
                            <div class="flex items-center gap-1 text-white justify-center">
                                <button class="bg-[#3B82F6] hover:bg-[#2563EB] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    
                                </button>
                                <button class="bg-red-500 hover:bg-[#DC2626] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                                    </svg>
                                    
                                </button>
                            </div>
                        </td>
                    </tr>

                    <tr class="">
                        <td class="flex items-center justify-center py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 "></td>
                        <td class="py-2">
                            <div class="image ">
                                <img src="https://avatars.dicebear.com/v2/initials/lonzo-steuber.svg" alt="" class="w-6 h-6 rounded-full
                                    ml-auto mr-auto block">
                            </div>
                        </td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">
                            <div class="bg-[#E5E7EB] w-24 h-3 rounded-xl">
                                <div class="row7 bg-blue-500 w-[1.5rem] h-3 rounded-xl" ></div>
                            </div>
                        </td>
                        <td class=" text-left py-2">Jan 8, 2021</td>
                        <td class=" text-left py-2">
                            <div class="flex items-center gap-1 text-white justify-center">
                                <button class="bg-[#3B82F6] hover:bg-[#2563EB] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    
                                </button>
                                <button class="bg-red-500 hover:bg-[#DC2626] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                                    </svg>
                                    
                                </button>
                            </div>
                        </td>
                    </tr>
                    <tr class="">
                        <td class="flex items-center justify-center py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 "></td>
                        <td class="py-2">
                            <div class="image ">
                                <img src="https://avatars.dicebear.com/v2/initials/jonathon-hahn.svg" alt="" class="w-6 h-6 rounded-full
                                    ml-auto mr-auto block">
                            </div>
                        </td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">
                            <div class="bg-[#E5E7EB] w-24 h-3 rounded-xl">
                                <div class="row8 bg-blue-500 w-20 h-3 rounded-xl" ></div>
                            </div>
                        </td>
                        <td class=" text-left py-2">Jan 8, 2021</td>
                        <td class=" text-left py-2">
                            <div class="flex items-center gap-1 text-white justify-center">
                                <button class="bg-[#3B82F6] hover:bg-[#2563EB] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    
                                </button>
                                <button class="bg-red-500 hover:bg-[#DC2626] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                                    </svg>
                                    
                                </button>
                            </div>
                        </td>
                    </tr>
                    <tr class="">
                        <td class="flex items-center justify-center py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 "></td>
                        <td class="py-2">
                            <div class="image ">
                                <img src="https://avatars.dicebear.com/v2/initials/ryley-wuckert.svg" alt="" class="w-6 h-6 rounded-full
                                    ml-auto mr-auto block">
                            </div>
                        </td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">
                            <div class="bg-[#E5E7EB] w-24 h-3 rounded-xl">
                                <div class="row9 bg-blue-500 w-16 h-3 rounded-xl" ></div>
                            </div>
                        </td>
                        <td class=" text-left py-2">Jan 8, 2021</td>
                        <td class=" text-left py-2">
                            <div class="flex items-center gap-1 text-white justify-center">
                                <button class="bg-[#3B82F6] hover:bg-[#2563EB] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    
                                </button>
                                <button class="bg-red-500 hover:bg-[#DC2626] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                                    </svg>
                                    
                                </button>
                            </div>
                        </td>
                    </tr>
                    <tr class="">
                        <td class="flex items-center justify-center py-4 accent-blue-500"><input type="checkbox" class="w-5 h-5 "></td>
                        <td class="py-2">
                            <div class="image ">
                                <img src="https://avatars.dicebear.com/v2/initials/sienna-hayes.svg" alt="" class="w-6 h-6 rounded-full
                                    ml-auto mr-auto block">
                            </div>
                        </td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">Felicita Yundt</td>
                        <td class=" text-left py-2">
                            <div class="bg-[#E5E7EB] w-24 h-3 rounded-xl">
                                <div class="row10 bg-blue-500 w-16 h-3 rounded-xl" ></div>
                            </div>
                        </td>
                        <td class=" text-left py-2">Jan 8, 2021</td>
                        <td class=" text-left py-2">
                            <div class="flex items-center gap-1 text-white justify-center">
                                <button class="bg-[#3B82F6] hover:bg-[#2563EB] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M2.036 12.322a1.012 1.012 0 010-.639C3.423 7.51 7.36 4.5 12 4.5c4.638 0 8.573 3.007 9.963 7.178.07.207.07.431 0 .639C20.577 16.49 16.64 19.5 12 19.5c-4.638 0-8.573-3.007-9.963-7.178z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    
                                </button>
                                <button class="bg-red-500 hover:bg-[#DC2626] p-2 rounded-sm flex items-center justify-center">
                                    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-4 h-4">
                                        <path stroke-linecap="round" stroke-linejoin="round" d="M14.74 9l-.346 9m-4.788 0L9.26 9m9.968-3.21c.342.052.682.107 1.022.166m-1.022-.165L18.16 19.673a2.25 2.25 0 01-2.244 2.077H8.084a2.25 2.25 0 01-2.244-2.077L4.772 5.79m14.456 0a48.108 48.108 0 00-3.478-.397m-12 .562c.34-.059.68-.114 1.022-.165m0 0a48.11 48.11 0 013.478-.397m7.5 0v-.916c0-1.18-.91-2.164-2.09-2.201a51.964 51.964 0 00-3.32 0c-1.18.037-2.09 1.022-2.09 2.201v.916m7.5 0a48.667 48.667 0 00-7.5 0" />
                                    </svg>
                                    
                                </button>
                            </div>
                        </td>
                    </tr>
                    
                </tbody>
            </table>
    </div>

</template>

<script>
    export default {
        name: 'Table',
        methods:{
            updatePage(){
                this.$emit('getPage','form')
            }
        },
    }
</script>

<style  scoped>
      table tr:nth-child(odd){background-color: #f3f6f6;}
  table thead tr{background-color: white;}

  table tr:hover {background-color: #F3F6F6;}
</style>