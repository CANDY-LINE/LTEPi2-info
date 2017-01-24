[🔙目次ページへ戻る](README.md)

既定の設定では、モデムが動作し、携帯電話のネットワークに接続している間は[LTEPi for D](https://www.candy-line.io/製品一覧/ltepi-for-d/)のLEDが点滅します。また、その時間間隔は0.4秒となっています。

これらの設定は、インストール後に`/opt/candy-line/ltepi2/environment`にある以下の箇所に定義されています。

```
# 1 for enabling LED blinking, 0 for disabling it
BLINKY=1
# Blinking interval in seconds, > 0 and <= 60
BLINKY_INTERVAL_SEC=0.4
```

`BLINKY`を0にすると、点滅をなくすことができます。ただし、常時点灯させることはできません。

`BLINKY_INTERVAL_SEC`には、点滅の時間間隔を秒で指定します。小数点を使うことができます。0より大きく、60以下の値を設定します。

「ルーターモード」と「モデムモード」では、点滅の方法が異なります。

- 「ルーターモード」 ... 点灯、消灯を交互に同じ時間間隔で繰り返します
- 「モデムモード」 ... 点滅を2回素早く行い、その後消灯が少し長く続きます。これを繰り返します


これらの設定を変更した場合は、ラズパイを再起動する必要があります。

---
© 2017 CANDY LINE, INC. [CC-BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)
