<template>
    <SectionedCard>
        <template #header>
            {{ title }}
        </template>
        <p>
            {{ when }}
        </p>
        <template #footer>
            <div class="space-y-4">
                <p>
                    {{ description }}
                </p>
                <div class="flex justify-end">
                    <RoundButton @click="$emit('register')">
                        Register
                    </RoundButton>
                </div>
            </div>
        </template>
    </SectionedCard>
</template>

<script setup>
defineProps({
    title: String,
    when: String,
    description: String
});
defineEmits(['register']);
import RoundButton from "@/components/RoundButton.vue"
import SectionedCard from "@/components/SectionedCard.vue";
</script>

