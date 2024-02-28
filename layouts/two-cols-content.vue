<template>
    <div class="slidev-layout w-full h-full">
        <slot />
        <div class="two-columns grid grid-cols-2 pt-15">
            <div class="col-left">
                <slot name="left" />
            </div>
            <div class="col-right">
                <slot name="right" />
            </div>
        </div>
    </div>

</template>