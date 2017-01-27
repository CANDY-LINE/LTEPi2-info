[🔙目次ページへ戻る](README.md)

モジュールが認識しているSIMの状態を表示します。 結果文字列の`state `には、以下の文字列が入ります。

1. `SIM_STATE_READY ` ... SIMが認識されている
1. `SIM_STATE_ABSENT ` ... SIMが認識されていない

```bash
pi@raspberrypi:~ $ sudo candy sim show
{
  "msisdn": "11111111111",
  "state": "SIM_STATE_READY",
  "imsi": "440111111111111"
}
```

* [APNの表示](APNの表示.md)
* [APNの設定](APNの設定.md)
* [ネットワーク状態の表示](ネットワーク状態の表示.md)
* [モデム情報の表示](モデム情報の表示.md)

---
© 2017 CANDY LINE INC. [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
