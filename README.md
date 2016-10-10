# z-countdown
倒计时


```js
    // var countdown = new Class(Date.now('2016-10-10 17:07:22'))
    var countdown = new Class(Date.now() + 5000)

    setTimeout(function () {
        countdown.pause()
    }, 800)

    setTimeout(function () {
        countdown.start()
    }, 2000)

    countdown
        .on('countdown', function (time) {
            console.log(time)
        })
        .on('end', function () {
            console.log('end')
        })
```