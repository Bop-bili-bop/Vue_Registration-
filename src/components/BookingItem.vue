<script setup>
import SectionedCard from '@/components/SectionedCard.vue';
import RoundButton from '@/components/RoundButton.vue';
defineProps({
    title: String,
    when: String,
    description: String
});
</script>

<template>
    <SectionedCard class="m-2">
        <div class="flex justify-between">
            <div>Booking to Vue Conference</div>
            <RoundButton variant="danger">
                Cancel
            </RoundButton>
        </div>
    </SectionedCard>
</template>