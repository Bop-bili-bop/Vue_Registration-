 <script setup>
import SectionedCard from '@/components/SectionedCard.vue';
import RoundButton from '@/components/RoundButton.vue';
defineProps({
    title: String,
    status: String
});
</script>

<template>
    <SectionedCard class="m-2">
        <div class="flex justify-between">
            <div>{{ title }}</div>
            <RoundButton variant="danger">
                Cancel
            </RoundButton>
        </div>
    </SectionedCard>
</template>