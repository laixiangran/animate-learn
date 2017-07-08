# Attention Seekers - 引起注意力的动画

## bounce - 弹跳

```
@keyframes bounce {
    /* 设置from, 20%, 53%, 80%, to时间点的样式 */
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

