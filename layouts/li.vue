<template>
    <div class="slidev-layout">
        <div class="my-auto grid grid-cols-2 gap-8">
            <!-- GM Default: tinted panels, no borders -->
            <div class="li-panel">
                <h1 class="li-heading">Learning intentions</h1>
                <slot name="li" />
            </div>
            <div class="li-panel">
                <h1 class="li-heading">Success criteria</h1>
                <p class="li-label">By the end of this lesson, students will be able to:</p>
                <slot name="sc" />
            </div>
        </div>
    </div>
</template>

<style scoped>
.li-panel {
    background: var(--gm-surface-tint);
    border-radius: var(--gm-radius-md);
    padding: var(--gm-space-6);
}

.li-heading {
    font-size: 22px;
    margin: 0 0 var(--gm-space-3) 0;
}

.li-label {
    font-size: 12px;
    font-weight: 600;
    line-height: 1.4;
    color: var(--gm-text-secondary);
    margin: 0 0 var(--gm-space-2) 0;
}
</style>
