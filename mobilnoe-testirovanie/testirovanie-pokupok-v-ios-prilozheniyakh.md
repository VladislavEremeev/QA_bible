# Тестирование покупок в iOS-приложениях

На iOS есть два варианта тестирования: классический, посредством Sandbox покупок, и новый способ локального тестирования покупок через Xcode (StoreKit local testing).

* [Sandbox тестирование](https://developer.apple.com/apple-pay/sandbox-testing/) - процесс несколько муторный и работает только на реальном девайсе. Чтобы тестировать в Sandbox, в самом начале надо завести аккаунт тестировщика на портале, связать его со своим устройством и после этого этого проверить все сценарии. Некоторые сценарии которых требуют очень большого количества манипуляций (refund, ask to buy, lifetime non-consumable покупки);
* [Тестирование в Xсode](https://developer.apple.com/documentation/xcode/testing-your-apps-in-xcode) стало доступным, начиная с Xcode 12 (iOS 14), и значительно упростило процесс тестирования. Во-первых, тестировать покупки в Xcode можно на раннем этапе, когда приложение не подключено к AppStore Connect. Во-вторых, для Xcode не нужно заводить дополнительных аккаунтов в AppStore, что сильно ускоряет процесс конфигурации тестов, особенно для lifetime non-consumable. В-третьих, локальное тестирование можно автоматизировать, что потенциально снижает шанс появления ошибок в коде. Более того, можно даже писать UI-тесты на пейволы и другие интерфейсы, где фигурируют покупки.

Однако некоторые вещи доступны только в Sandbox. Например, использовать таблицу цен с автоматической конвертацией на разные валюты можно только в AppStore. Также валидация покупок (receipt validation) в обычном виде уже не работает - локальные покупки валидируются через Xcode, и этот механизм ложится на плечи разработчика. В остальном Xcode покрывает большинство сценариев и задач тестирования.

Источники:

* [iOS in-app purchases, часть 4: локальное тестирование покупок в XCode](https://habr.com/ru/company/adapty/blog/571960/)

Доп. материал:

* [Testing In-App Purchases in Xcode](https://developer.apple.com/documentation/storekit/original\_api\_for\_in-app\_purchase/testing\_in-app\_purchases\_in\_xcode)
* [Test in-app purchases in Sandbox](https://help.apple.com/app-store-connect/#/dev7e89e149d)
* [In-app purchase types](https://help.apple.com/app-store-connect/#/dev3cd978dbd)
* [In-app purchase statuses](https://help.apple.com/app-store-connect/#/dev840c56fb6)
* [Auto-renewable subscription information](https://help.apple.com/app-store-connect/#/dev7f2d6b652)
