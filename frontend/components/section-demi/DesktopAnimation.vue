<template>
  <div class="relative">
        <img src="../../assets/img/window.png" alt="Fenêtre" class="w-[600px]">
        <img src="../../assets/img/window-scroll.png" alt="Scrollbar" class="scrollbar absolute right-[80px] bottom-[150px] w-[24px]">
        <img src="../../assets/img/icons/cursor.png" alt="Cursor" class="cursor absolute right-[100px] bottom-[150px] w-[26px]">
        <img src="../../assets/img/window-text.png" alt="Texte" class="text absolute right-[130px] bottom-[200px] w-[125px]">
        <img src="../../assets/img/window-text.png" alt="Texte" class="text absolute right-[130px] bottom-[375px] w-[125px]">
        <div class="absolute top-[22px] left-[150px] bg-[#F2F1ED] w-[375px] h-[50px] z-10"></div>
        <div class="component-desktop absolute top-[50px] right-[275px] w-[175px] h-[175px]">
            <div class="relative h-full">
                <img src="../../assets/img/window-component.png" alt="Component" class="w-[175px] absolute top-[50%] left-[50%] -translate-y-1/2 -translate-x-1/2">
                <img src="../../assets/img/icons/idea.svg" alt="Idee" class="w-[125px] absolute top-[50%] left-[50%] -translate-y-1/2 -translate-x-1/2">
            </div>
        </div>
        <div class="component-desktop absolute top-[225px] right-[275px] w-[175px] h-[175px]">
            <div class="relative h-full">
                <img src="../../assets/img/window-component.png" alt="Component" class="w-[175px] absolute top-[50%] left-[50%] -translate-y-1/2 -translate-x-1/2">
                <img src="../../assets/img/icons/objects.svg" alt="Objet" class="w-[125px] absolute top-[50%] left-[50%] -translate-y-1/2 -translate-x-1/2">
            </div>
        </div>
    </div>
</template>

<style>
.component-desktop {
    animation: desktop-animation 3s ease-in-out infinite alternate;
}
.scrollbar {
    animation: scroll-animation 3s ease-in-out infinite alternate;
}
.cursor {
    animation: cursor-animation 3s ease-in-out infinite alternate;
}
.text {
    animation: text-animation 3s ease-in-out infinite alternate;
}

@keyframes component-mobile-animation {
    from {
        -webkit-transform: translateY(-10%);
        transform: translateY(-10%);
    }
    to {
        -webkit-transform: translateY(10%);
        transform: translateY(10%);
    }
}
@keyframes desktop-animation {
    0% {
        -webkit-transform: translateY(-25%);
        transform: translateY(-25%);
    }
    30% {
        -webkit-transform: translateY(-25%);
        transform: translateY(-25%);
    }
    80% {
        -webkit-transform: translateY(20%);
        transform: translateY(20%);
    }
    100% {
        -webkit-transform: translateY(20%);
        transform: translateY(20%);
    }
}
@keyframes scroll-animation {
    0% {
        -webkit-transform: translateY(30%);
        transform: translateY(30%);
    }
    30% {
        -webkit-transform: translateY(30%);
        transform: translateY(30%);
    }
    80% {
        -webkit-transform: translateY(-75%);
        transform: translateY(-75%);
    }
    100% {
        -webkit-transform: translateY(-75%);
        transform: translateY(-75%);
    }
}
@keyframes cursor-animation {
    0% {
        -webkit-transform: translate(-35px, 30%);
        transform: translate(-35px, 30%);
    }
    30% {
        -webkit-transform: translate(30px, 30%);
        transform: translate(30px, 30%);
    }
    31% {
        -webkit-transform: translate(30px, 30%) scale(.7);
        transform: translate(30px, 30%) scale(.7);
    }
    80% {
        -webkit-transform: translate(30px, -425%) scale(.7);
        transform: translate(30px, -425%) scale(.7);
    }
    100% {
        -webkit-transform: translate(30px, -425%) scale(.7);
        transform: translate(30px, -425%) scale(.7);
    }
}
@keyframes text-animation {
    0% {
        -webkit-transform: translateY(-50%);
        transform: translateY(-50%);
    }
    30% {
        -webkit-transform: translateY(-50%);
        transform: translateY(-50%);
    }
    80% {
        -webkit-transform: translateY(125%);
        transform: translateY(125%);
    }
    100% {
        -webkit-transform: translateY(125%);
        transform: translateY(125%);
    }
}
</style>

