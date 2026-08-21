<template>
    <div class="flex items-center gap-6 max-lg:flex-col lg:justify-between">
        <div class="flex flex-col gap-6 w-full lg:w-[55%]">
            <div class="flex items-center gap-2 rounded-full px-3 py-1.5 border border-[#6D56E83F] w-fit bg-[#6d56e824]">
                <div class="w-1.5 h-1.5 rounded-full bg-[#8570f5]"></div>
                <p class="text-[12px] leading-[100%] font-semibold text-[#8570f5]">ИИ-НАВИГАТОР ПО ЦЕЛЯМ</p>
            </div>
            <h1 class="text-[#edeaf5]">Разбей любую цель <span class="text-[#8570f5]">на конкретные шаги</span></h1>
            <p class="text-base text-[#7e7c96]">
                APEX анализирует твою цель и строит план: подцели, задачи, дедлайны. <br>
                ИИ-коуч помогает не сбиться с курса — от уборки до запуска стартапа.
            </p>
            <div class="flex item-center gap-4 max-md:flex-col">
                <NuxtLink to="/" class="w-fit max-md:w-full flex items-center gap-1.5 bg-[#6d56e8] text-white px-4 py-2 rounded-md transition-all duration-300 font-semibold hover:-translate-y-px hover:bg-[#8570f5]">
                    <span>Начать</span>
                    <Icon class="text-xl" name="ic:outline-arrow-right-alt"/>
                </NuxtLink>
                <NuxtLink to="/" class="w-fit max-md:w-full flex items-center gap-1.5 text-[#7e7c96] border border-[#FFFFFF21] px-4 py-2 rounded-md transition-all duration-300 font-semibold hover:border-[#48465e] hover:text-[#edeaf5] hover:bg-[#18181f]">
                    <span>Как это работает</span>
                </NuxtLink>
            </div>
        </div>
        <div class="w-full lg:w-[45%] rounded-2xl bg-[#111118] border border-[#FFFFFF21]">
            <div class="flex items-center gap-4 p-4 border-b border-[#FFFFFF12]">
                <div class="flex items-center gap-1.5">
                    <div class="w-2 h-2 rounded-full bg-[#ef5757]"></div>
                    <div class="w-2 h-2 rounded-full bg-[#f5845a]"></div>
                    <div class="w-2 h-2 rounded-full bg-[#10d9a0]"></div>
                </div>
                <p class="text-xs text-[#48465e]">цель / запустить-продукт</p>
            </div>
            <div class="flex flex-col gap-6 p-4">
                <div class="flex items-center justify-between">
                    <div class="flex flex-col gap-1">
                        <p class="text-base text-[#edeaf5] font-semibold">Запустить SaaS-продукт</p>
                        <p class="text-xs text-[#7e7c96]">Цель: $3 000 MRR · 31 дек 2026</p>
                    </div>
                    <p class="text-xl font-semibold text-[#8570f5]">35%</p>
                </div>
                <div class="w-full h-1 rounded-full bg-[#18181f] -mt-2">
                    <div class="w-[35%] h-1 rounded-full bg-[#6d56e8]"></div>
                </div>
                <div class="flex flex-col gap-2">
                    <div class="flex flex-col gap-1">
                        <div class="flex items-center justify-between text-xs text-[#7e7c96] font-medium">
                            <p>Валидация идеи</p>
                            <p>4/4</p>
                        </div>
                        <div class="w-full h-1 rounded-full bg-[#18181f]">
                            <div class="w-full h-1 rounded-full bg-[#10d9a0]"></div>
                        </div>
                    </div>
                    <div class="flex flex-col gap-1">
                        <div class="flex items-center justify-between text-xs text-white font-medium">
                            <p>Сборка MVP</p>
                            <p>2/5</p>
                        </div>
                        <div class="w-full h-1 rounded-full bg-[#18181f]">
                            <div class="w-2/5 h-1 rounded-full bg-[#6d56e8]"></div>
                        </div>
                    </div>
                    <div class="flex flex-col gap-1">
                        <div class="flex items-center justify-between text-xs text-white font-medium">
                            <p>Инфраструктура</p>
                            <p>1/4</p>
                        </div>
                        <div class="w-full h-1 rounded-full bg-[#18181f]">
                            <div class="w-1/4 h-1 rounded-full bg-[#6d56e8]"></div>
                        </div>
                    </div>
                    <div class="flex flex-col gap-1">
                        <div class="flex items-center justify-between text-xs text-white font-medium">
                            <p>Запуск</p>
                            <p>0/4</p>
                        </div>
                        <div class="w-full h-1 rounded-full bg-[#18181f]">
                            <div class="w-0 h-1 rounded-full bg-[#6d56e8]"></div>
                        </div>
                    </div>
                </div>
                <div class="flex gap-2 p-2 rounded-lg">
                    <Icon class="text-3xl text-[#6d56e8]" name="hugeicons:artificial-intelligence-04"/>
                    <p class="text-xs text-[#7e7c96]">                     
                        Выпусти MVP до того, как добавлять фичи. Главный риск сейчас — строить без обратной связи от пользователей.
                    </p>
                </div>
            </div>
        </div>
    </div>
    <div class="flex flex-col gap-8">
        <div class="flex flex-col gap-1">
            <p class="text-sm text-[#7e7c96] font-medium uppercase">Процесс</p>
            <h2 class="text-[#edeaf5]">Как работает APEX</h2>
        </div>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-1">
            <div class="rounded-xl px-8 py-6 flex flex-col gap-6 border border-[#FFFFFF12] even:bg-[#18181f] odd:bg-[#111118]" v-for="step in steps">
                <p class="text-sm text-[#7e7c96] font-medium">{{ step.n }}</p>
                <div class="flex items-center justify-center w-10 h-10 rounded-md bg-[#6D56E824]">
                    <div class="w-4 h-4 rounded-full bg-[#8570f5]"></div>
                </div>
                <p class="text-base font-bold text-[#edeaf5]">{{ step.title }}</p>
                <p class="text-[17px] leading-[125%] text-[#7e7c96]">{{ step.desc }}</p>
            </div>
        </div>
    </div>
</template>
 
<script setup>
/* steps */
const steps = [
  {
    n: '01',
    title: 'Опиши цель',
    desc: 'В свободной форме — от «разобрать завалы на рабочем столе» до «запустить продукт с первыми клиентами».',
  },
  {
    n: '02',
    title: 'ИИ строит план',
    desc: 'Цель разбивается на подцели и конкретные задачи с дедлайнами. Никакого пустого листа.',
  },
  {
    n: '03',
    title: 'Выполняй и адаптируйся',
    desc: 'Отмечай задачи, общайся с коучем, следи за прогрессом. План живёт вместе с тобой.',
  },
]
</script>