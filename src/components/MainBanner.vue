<template>
    <div class="container-width mb-10 md:my-16 flex flex-col md:flex-row items-center justify-between relative">
        <img src="../assets/mainbannershadow.png" class="absolute" loading="lazy" alt="Main Banner Shadow">
        <div class="w-full md:w-1/2 ml-5">
            <img src="../assets/mainbanner.png" loading="lazy" alt="Main Banner">
        </div>

        <div class="w-full md:w-1/2 space-y-6 flex flex-col items-end">
            <h2 class="text-right text-2xl md:text-[30px] xl:text-[55px] font-bold leading-relaxed">
                <span class="text-primary text-2xl md:text-[30px] xl:text-[60px]">سهولة الاختبار العام</span>
                <br>
                رحلة متكاملة نحو أعلى الدرجات
            </h2>

            <div class="flex items-center flex-wrap gap-2 md:gap-4 justify-end">
                <BadgeItem v-for="badge in badges" :key="badge.id" :text="badge.text" />
            </div>

            <p class="font-medium text-base md:text-xl text-right text-[#666666]"> للمعلمين والخريجين الطامحين للتميز
                محتوى تعليمي شامل من ست محطات رئيسية</p>

            <div class="flex flex-wrap !justify-end 2xl:justify-start gap-x-20 gap-y-5 items-end text-right">
                <FeatureItem v-for="feature in features" :key="feature.id" :text="feature.text" />
            </div>
        </div>
    </div>
</template>

<script setup>
import { ref } from 'vue'
import BadgeItem from './BadgeItem.vue'
import FeatureItem from './FeatureItem.vue'

const badges = ref([
    { id: 1, text: 'لغـــــوي' },
    { id: 2, text: 'لفــــظي' },
    { id: 3, text: 'كــــــمي' }
])

const features = ref([
    { id: 1, text: 'امتحانات تفاعلية ومتطورة' },
    { id: 2, text: 'دورات معتمدة من هيئة تقويم التعليم' },
    { id: 3, text: 'متابعة مستمرة للتقدم' },
    { id: 4, text: 'التاهل للحصول على الرخصة المهنية' }
])
</script>