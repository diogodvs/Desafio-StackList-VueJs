<template>

    <div class="flex place-content-around w-[45rem] m-auto ">

        <div class="flex bg-black-400 px-2 py-2 rounded-lg absolute">

            <button class="px-2 flex" @click="$i18n.locale = locales[0]">

                <img class="px-2" src="../assets/bra.icon.svg" alt="">
                {{$t('portuguese')}}

            </button>

        </div>
       
        <div class="flex bg-black-400 px-2 py-2 rounded-lg">
            <button class="px-2 flex" @click="$i18n.locale = locales[1]">
               
                <img class="px-2" src="../assets/eua.icon.svg" alt="">
                {{$t('english')}}

            </button>

        </div>

        <div class="flex bg-black-400 px-2 py-2 rounded-lg">

            <button class="px-2 flex" @click="$i18n.locale = locales[2]">

                <img class="px-2" src="../assets/spa.icon.svg" alt="">
                {{$t('spanish')}}

            </button>

        </div>
       
    </div>
</template>

<script>
 import { useI18n } from 'vue-i18n'

    export default {
        name: 'LocaleSwitcher',
        setup() {
            const { t } = useI18n({
            inheritLocale: true,
            useScope: 'local'
            })
            
            return { t }
        },
        
        data() {
            return {
                locales: ["pt", "en", "es"],
            }
        }
    }
</script>