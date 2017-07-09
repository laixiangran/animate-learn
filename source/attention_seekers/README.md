# Attention Seekers - 引起注意力的动画

## bounce - 弹跳

```css
@keyframes bounce {

    /* 设置from(0%), 20%, 53%, 80%, to(100%)时间点的样式 */
    from, 20%, 53%, 80%, to {
        /* 设置对象动画的过渡类型为特定的cubic-bezier（贝塞尔曲线）类型，4个数值分别为0.215, 0.610, 0.355, 1.000 */
        animation-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
        /* 指定对象的3D位移。X轴，Y轴，Z轴位移分别为0，0，0 */
        transform: translate3d(0, 0, 0);
    }

    /* 设置40%, 43%时间点的样式 */
    40%, 43% {
        /* 设置对象动画的过渡类型为特定的cubic-bezier（贝塞尔曲线）类型，4个数值分别为0.755, 0.050, 0.855, 0.060 */
        animation-timing-function: cubic-bezier(0.755, 0.050, 0.855, 0.060);
        /* 指定对象的3D位移。X轴，Y轴，Z轴位移分别为0，-30px，0 */
        transform: translate3d(0, -30px, 0);
    }

    /* 设置70%时间点的样式 */
    70% {
        /* 设置对象动画的过渡类型为特定的cubic-bezier（贝塞尔曲线）类型，4个数值分别为0.755, 0.050, 0.855, 0.060 */
        animation-timing-function: cubic-bezier(0.755, 0.050, 0.855, 0.060);
        /* 指定对象的3D位移。X轴，Y轴，Z轴位移分别为0，-15px，0 */
        transform: translate3d(0, -15px, 0);
    }

    /* 设置90%时间点的样式 */
    90% {
        /* 指定对象的3D位移。X轴，Y轴，Z轴位移分别为0，-4px，0 */
        transform: translate3d(0, -4px, 0);
    }
}

.bounce {
    animation-name: bounce; /* 对象应用的动画名称 */
    transform-origin: center bottom; /* 设置对象转换的原点位置 */
}
```

## flash - 闪动

```css
@keyframes flash {

    /* 设置from(0%), 50%, to(100%)时间点的样式 */
    from, 50%, to {
        opacity: 1; /* 设置透明度为1 */
    }

    /* 设置25%, 75%时间点的样式 */
    25%, 75% {
        opacity: 0; /* 设置透明度为0 */
    }
}

.flash {
    animation-name: flash;
}
```

## headShake - 摇头

```css
@keyframes headShake {

    0% {
        /* 设置对象X轴（水平方向）的平移为0 */
        transform: translateX(0);
    }

    6.5% {
        /* 设置对象X轴（水平方向）的平移为-6px，设置对象在y轴上的旋转角度为-9deg */
        transform: translateX(-6px) rotateY(-9deg);
    }

    18.5% {
        /* 设置对象X轴（水平方向）的平移为5px，设置对象在y轴上的旋转角度为7deg */
        transform: translateX(5px) rotateY(7deg);
    }

    31.5% {
        /* 设置对象X轴（水平方向）的平移为-3px，设置对象在y轴上的旋转角度为-5deg */
        transform: translateX(-3px) rotateY(-5deg);
    }

    43.5% {
        /* 设置对象X轴（水平方向）的平移为2px，设置对象在y轴上的旋转角度为3deg */
        transform: translateX(2px) rotateY(3deg);
    }

    50% {
        /* 设置对象X轴（水平方向）的平移为0px */
        transform: translateX(0);
    }
}

.headShake {
    animation-timing-function: ease-in-out; /* 设置过渡类型由慢到快再到慢 */
    animation-name: headShake;
}
```

## jello - 果冻

```css
@keyframes jello {
    from, 11.1%, to {
        transform: none;
    }

    22.2% {
        /* 设置对象X轴的（水平方向）扭曲为-12.5deg，对象Y轴的（水平方向）扭曲为-12.5deg */
        transform: skewX(-12.5deg) skewY(-12.5deg);
    }

    33.3% {
        /* 设置对象X轴的（水平方向）扭曲为6.25deg，对象Y轴的（水平方向）扭曲为6.25deg */
        transform: skewX(6.25deg) skewY(6.25deg);
    }

    44.4% {
        /* 设置对象X轴的（水平方向）扭曲为-3.125deg，对象Y轴的（水平方向）扭曲为-3.125deg */
        transform: skewX(-3.125deg) skewY(-3.125deg);
    }

    55.5% {
        /* 设置对象X轴的（水平方向）扭曲为1.5625deg，对象Y轴的（水平方向）扭曲为1.5625deg */
        transform: skewX(1.5625deg) skewY(1.5625deg);
    }

    66.6% {
        /* 设置对象X轴的（水平方向）扭曲为-0.78125deg，对象Y轴的（水平方向）扭曲为-0.78125deg */
        transform: skewX(-0.78125deg) skewY(-0.78125deg);
    }

    77.7% {
        /* 设置对象X轴的（水平方向）扭曲为0.390625deg，对象Y轴的（水平方向）扭曲为0.390625deg */
        transform: skewX(0.390625deg) skewY(0.390625deg);
    }

    88.8% {
        /* 设置对象X轴的（水平方向）扭曲为-0.1953125deg，对象Y轴的（水平方向）扭曲为-0.1953125deg */
        transform: skewX(-0.1953125deg) skewY(-0.1953125deg);
    }
}

.jello {
    animation-name: jello;
    transform-origin: center; /* 设置对象转换的原点位置为center */
}
```

