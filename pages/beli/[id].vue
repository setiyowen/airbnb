<template>
    <div class="flex justify-center bg-gradient-to-r from-cyan-500 to-blue-500 h-screen">
        <div class="mx-auto grid max-w-screen-2xl grid-cols-1 md:grid-cols-2">
            <div class="bg-gray-50 py-12 md:py-24 border-[2px]">
                <div class="mx-auto max-w-lg space-y-8 px-4 lg:px-8">
                    <div class="flex items-center gap-4">
                        <img src="/img/logoairbnb.png" class="h-10 w-10 rounded-full bg-blue-500">
                        <h2 class="font-medium text-gray-900">Airbnb</h2>
                    </div>

                    <div>
                        <p class="text-2xl font-medium tracking-tight text-gray-900">
                            $46.78
                        </p>

                        <p class="mt-1 text-sm text-gray-600">For the purchase of</p>
                    </div>

                    <div>
                        <div class="flow-root">
                            <ul class="-my-4 divide-y divide-gray-100">
                                <li class="flex items-center gap-4 py-4">
                                    <img src="/img/ip1.jpg" class="h-16 w-16 rounded object-cover" />

                                    <div>
                                        <h3 class="text-sm text-gray-900">{{ product.title }}</h3>

                                        <dl class="mt-0.5 space-y-px text-[10px] text-gray-600">
                                            <div>
                                                <dt class="inline">Description:</dt>
                                                <dd class="inline">{{ product.description }}</dd>
                                            </div>

                                            <div>
                                                <dt class="inline">Color:</dt>
                                                <dd class="inline">White</dd>
                                            </div>
                                        </dl>
                                    </div>
                                </li>

                                <li class="flex items-center gap-4 py-4">
                                    <img src="/img/ip2.jpg" class="h-16 w-16 rounded object-cover" />

                                    <div>
                                        <h3 class="text-sm text-gray-900">{{ product.title }}</h3>

                                        <dl class="mt-0.5 space-y-px text-[10px] text-gray-600">
                                            <div>
                                                <dt class="inline">Description:</dt>
                                                <dd class="inline">{{ product.description }}</dd>
                                            </div>

                                            <div>
                                                <dt class="inline">Color:</dt>
                                                <dd class="inline">White</dd>
                                            </div>
                                        </dl>
                                    </div>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>

            <div class="bg-white py-12 md:py-24">
                <div class="mx-auto max-w-lg px-4 lg:px-8">
                    <form class="grid grid-cols-6 gap-4">
                        <div class="col-span-3">
                            <label for="FirstName" class="block text-xs font-medium text-gray-700">
                                Nama Depan
                            </label>

                            <input type="text" id="FirstName"
                                class="block mt-1 w-full text-sm text-gray-900 bg-gray-50 rounded-md border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" />
                        </div>

                        <div class="col-span-3">
                            <label for="LastName" class="block text-xs font-medium text-gray-700 ">
                                Nama Belakang
                            </label>

                            <input type="text" id="LastName"
                                class="mt-1 w-full text-sm text-gray-900 bg-gray-50 rounded-md border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" />
                        </div>

                        <div class="col-span-6">
                            <label for="Email" class="block text-xs font-medium text-gray-700">
                                Email
                            </label>

                            <input type="email" id="Email"
                                class="mt-1 w-full text-sm text-gray-900 bg-gray-50 rounded-md border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" />
                        </div>

                        <div class="col-span-6">
                            <label for="Phone" class="block text-xs font-medium text-gray-700">
                                No handphone
                            </label>

                            <input type="tel" id="Phone"
                                class="mt-1 w-full text-sm text-gray-900 bg-gray-50 rounded-md border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" />
                        </div>

                        <fieldset class="col-span-6">
                            <legend class="block text-sm font-medium text-gray-700">
                                Card Details
                            </legend>

                            <div class="mt-1 -space-y-px rounded-md bg-white shadow-sm">
                                <div>
                                    <label for="CardNumber" class="sr-only"> Card Number </label>

                                    <input type="text" id="CardNumber" placeholder="Card Number"
                                        class="relative mt-1 w-full text-sm text-gray-900 bg-gray-50 rounded-md border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" />
                                </div>

                                <div class="flex">
                                    <div class="flex-1">
                                        <label for="CardExpiry" class="sr-only"> Card Expiry </label>

                                        <input type="text" id="CardExpiry" placeholder="Expiry Date"
                                            class="relative w-full text-sm text-gray-900 bg-gray-50 rounded-md border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" />
                                    </div>

                                    <div class="-ms-px flex-1">
                                        <label for="CardCVC" class="sr-only"> Card CVC </label>

                                        <input type="text" id="CardCVC" placeholder="CVC"
                                            class="relative w-full text-sm text-gray-900 bg-gray-50 rounded-md border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" />
                                    </div>
                                </div>
                            </div>
                        </fieldset>

                        <fieldset class="col-span-6">
                            <legend class="block text-sm font-medium text-gray-700">
                                Billing Address
                            </legend>
                            <!-- massage -->
                            <label for="message"
                                class="block mb-2 text-sm font-medium text-gray-900 dark:text-white"></label>
                            <textarea id="message" rows="4"
                                class="block p-2.5 w-full text-sm text-gray-900 bg-gray-50 rounded-lg border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 "
                                placeholder="Write your Address..."></textarea>
                            <div class="mt-1 -space-y-px rounded-md bg-white shadow-sm ">
                                <div>
                                    <label for="Country" class="sr-only">Country</label>

                                    <select id="Country"
                                        class="relative  w-full text-sm text-gray-900 bg-gray-50 rounded-md border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 ">
                                        <option>England</option>
                                        <option>Indonesia</option>
                                        <option>Malaysia</option>
                                        <option>France</option>
                                        <option>Singapore</option>
                                        <option>Japan</option>
                                    </select>
                                </div>

                                <div>
                                    <label class="sr-only" for="PostalCode"> ZIP/Post Code </label>

                                    <input type="text" id="PostalCode" placeholder="ZIP/Post Code"
                                        class="relative w-full text-sm text-gray-900 bg-gray-50 rounded-md border border-gray-300 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400" />
                                </div>
                            </div>
                        </fieldset>
                        <!-- col-span-6 -->
                    </form>
                    <div class=" mt-3 flex justify-between ">
                        <NuxtLink :to="`/`" :key="product.id">
                            <p
                                class="inline-block text-sm text-gray-500 underline underline-offset-4 transition hover:text-gray-600  ">
                                Lanjut Belanja</p>
                        </NuxtLink>
                        <button
                            class="inline-block rounded bg-gray-700 px-12 py-1 text-sm text-gray-100 transition hover:bg-gray-600 ">Pay
                            Now</button>
                        <!-- popup -->

                    </div>

                </div>
            </div>
        </div>
    </div>
</template>

<script setup>

const { id } = useRoute().params
const uri = 'https://dummyjson.com/products/' + id

// fetch
const { data: product } = await useFetch(uri)

</script>