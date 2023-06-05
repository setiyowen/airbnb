<template>
    <div class="p-2 place-content-center">
        <div class="">
            <div class="max-w-sm rounded overflow-hidden shadow-lg">
                <div class="mb-[10px]">
                    <img src="/img/lego1.png" class="w-[290px] h-[200px] rounded-md">
                </div>
                <div>
                    <div class="flex-none">
                        <img src="/img/lego1.png" class="w-[290px] h-[200px] rounded-md">
                        <div class="flex">
                            <p
                                class="font-semibold mt-[8px] border-[1px] border-slate-800 max-w-sm text-base py-2 px-3 rounded-sm text-slate-800">
                                {{ tag }}</p>
                            <p class="text-base text-slate-800 items-center pl-[13px] mt-[20px] w-[120px]">{{ tag2 }}</p>
                            <div class="flex">
                                <img src="/img/logoairbnb.png"
                                    class="w-[10px] h-[10px] items-center pl-1 mt-[26px] ml-[0px]">
                                <p class="text-xs text-cyan-600 text-right mt-[22px] ml-[4px]">{{ tag3 }}</p>
                            </div>

                        </div>
                        <p class="text-sm text-gray-500 mt-[8px]">{{ tag4 }}</p>
                    </div>
                </div>
            </div>


        </div>
    </div>
</template>

<script setup>
const props = defineProps({
    // title: String,
    subheading: String,
    text: String,
    tag: String,
    tag2: String,
    tag3: String,
    tag4: String,
})

</script>