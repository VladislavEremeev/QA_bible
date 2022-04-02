# Каким образом тестировщик получает приложение на тест?

**Android**:

* Разработчик скинет .apk :) или .aab, который нужно разархивировать;
* Из CI-агента. Тот же Jenkins/TeamCity может присылать ссылку на билд в tg-канал или можно забрать его вручную;
* Сбилдить в Android Studio самому из нужной ветки;
* [Открытые и закрытые бета-тестирования приложений в Google Play](https://support.google.com/googleplay/android-developer/answer/9845334?hl=ru);

**iOS**:

* сбилдить в Xcode;
* внутреннее и внешнее тестирование в [TestFlight](https://testflight.apple.com);
* сервис [tiny.app.link](https://getappbox.com)

Доп. материал:

* [Visual Studio App Center](https://appcenter.ms)
