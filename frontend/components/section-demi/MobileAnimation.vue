<template>
<div class="-bottom-20 left-0 mobile w-[250px]">
    <div class="relative">
        <img src="../../assets/img/window-tel.png" alt="Telephone">
        <div class="component-mobile absolute top-20 left-[22px] w-[175px] h-[175px]">
            <div class="relative h-full">
                <img src="../../assets/img/window-component.png" alt="Component" class="w-[175px] absolute top-[50%] left-[50%] -translate-y-1/2 -translate-x-1/2">
                <img src="../../assets/img/icons/teamwork.svg" alt="Teamwork" class="w-[100px] absolute top-[50%] left-[50%] -translate-y-1/2 -translate-x-1/2">
            </div>
        </div>
    </div>
</div>  
</template>

<style>

.mobile {
    animation: mobile-animation 2s ease-in infinite alternate;
}
.component-mobile {
    animation: component-mobile-animation 2s ease-in infinite alternate;
}
@keyframes mobile-animation {
    from {
        -webkit-transform: translateY(-4%);
        transform: translateY(-4%);
    }
    to {
        -webkit-transform: translateY(2%);
        transform: translateY(2%);
    }
}
</style>