<template>
    <div class="slidev-layout">
        <div class="my-auto">
            <div class="border border-gray-400 ring-0 p-4 rounded-lg">
                <h1 class="text-4xl pt-2 text-green-600"> Learning Intentions</h1>
                <slot name="li"/>
            </div>
            <div class="border border-gray-400 ring-0 p-4 rounded-lg mt-6">
                <h1 class="text-4xl pt-2 pb-2 text-indigo-600">Success Criteria</h1>
                <h2 class="text-xl text-gray-600 italic">By the end of this lesson, students will be able to:</h2>
                <slot name="sc"/>
            </div>
        </div>
    </div>
</template>
