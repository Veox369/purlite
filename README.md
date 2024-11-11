# purlite
نسخه سبک پورکاو تحت نام پورلایت.مناسب خانواده ها و کسانی که میخان درگیر تنظیمات اضافه نشن.
این نسخه فقط دارای یک دکمه خاموش و روشن کردن هست.همچنین  خاموش  و روشن  کردن توسط دکمه نوار کشویی بالا و ویجت هم میسر هست.


<center>
  <picture>
   <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://github.com/davudsedft/purlite/blob/main/link/pur1.jpg" width="200px"  >
</picture>
 <picture>
   <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://github.com/davudsedft/purlite/blob/main/link/pur2.jpg" width="200px"  >
</picture>
 <picture>
   <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://github.com/davudsedft/purlite/blob/main/link/pur3.jpg" width="200px"  >
</picture>
</center>

برای خروجی گرفتن از کتابخانه گو
go v 1.22

cd v2ray/libs

go mod tidy

go install golang.org/x/mobile/cmd/gomobile@latest

go install golang.org/x/mobile/cmd/gobind@latest

go get golang.org/x/mobile/cmd/gobind

go get golang.org/x/mobile/cmd/gomobile

go get golang.org/x/mobile

gomobile init

gomobile bind -ldflags '-s -w' -o purlite.aar -androidapi 21 -target android .




طریقه ساخت apk
وارد پوشه root  پروژه شده و در cmd دستور 
cd /purlite/

```sh
gradlew assembleDebug
```
و در لینوکس در ترمینال 
```sh
./gradlew assembleDebug
```
خروجی در پوشه 
app/build/outputs/apk/release



برای نسخه ریلیس باید در گریدل مشخصات keystore خودتون و وارد فایل گریدل کنین یا نسخه ریلیس را از همینجا دانلود کنین

دستور cmd ویندوز برای خروجی نسخه ریلیس 


```sh
gradlew assembleRelease
```

دستور ترمینال در لینوکس ./ در اول دستور قرار بدین



```sh
./gradlew assembleRelease
```




## Credits
- https://github.com/xtls/xray-core
- https://github.com/2dust/AndroidLibXrayLite
- https://github.com/dev7dev/AndroidLibXrayLite
- https://github.com/gvcgo/vpnparser


