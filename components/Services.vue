<template>
    <section id="service" class="container mx-auto">
        <SectionHeading text="what i will do">Services</SectionHeading>
        <!-- space-x-8 -->
        <div
            class="flex flex-col lg:flex-row space-y-4 lg:space-y-0 lg:space-x-4 max-w-[1100px] mx-auto"
        >
            <ServicesCard
                title="Website Development"
                :items="items.websiteDev"
            />
            <ServicesCard title="Font End Development" :items="items.fontEnd" />
            <ServicesCard
                title="Full Stack Development"
                :items="items.backEnd"
            />
        </div>
    </section>
</template>
<script setup lang="ts">
const items = {
    websiteDev: [
        'Website With HTML, CSS, Javascript',
        'MultiPage Static Website',
        'Landing Page',
    ],
    fontEnd: [
        'Client Site Web App',
        'ECommerce Site Development',
        'React, Vue',
        'Server Side Render App: Next, Nuxt',
        'Authentication, Authorization',
    ],
    backEnd: [
        'Complete Web App',
        'Api Building',
        'Database Integration',
        'Microservices',
    ],
};
</script>
