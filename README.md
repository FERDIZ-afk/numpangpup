**Deploy dulu**

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?template=https://github.com/frmdeveloper/numpangpup)

___
**Fungsi:** Numpang/kontrol puppeteer dari perangkat lain<br>
___
cara menggunakan di JS
```
const puppeteer = require('puppeteer-core')
(async() => {
  urlws = "ws://blabla"
  var browser = await puppeteer.connect({ browserWSEndpoint: urlws })
  var page = await browser.newPage()
  await page.setViewport({ width: 1280, height: 720 })
  await page.goto('https://google.com')
  await page.screenshot({ path: `./screenshot.png` })
  await page.close()
  browser.dicsonnect()
})()
```
___
#### Cara lain lihat google
