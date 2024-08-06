# SIM7080 Stamp Module

<img src="https://github.com/akita11/SIM7080module/blob/main/SIM7080mod_f.jpg" width="240px">

<img src="https://github.com/akita11/SIM7080module/blob/main/SIM7080mod_b.jpg" width="240px">

M5Stack社の[M5Stamp SIM7080G搭載CAT-Mモジュール](https://www.switch-science.com/products/8194)をM5Stackにスタックできるモジュールにするための基板とフレームです。フレームにはアンテナを固定できる穴があいています。※「M5Stamp SIM7080G搭載CAT-Mモジュール（SIM7080モジュール）」は別途用意して下さい。





## 組み立て

以下のいずれかの方法で、本ボードにSIM7080モジュールをはんだ付けします。アンテナのコネクタは、いずれの場合も、フレームの穴に固定します。


### その1(SIMスロットがモジュール内にある向き）

<img src="https://github.com/akita11/SIM7080module/blob/main/SIM7080mod_usage1.jpg" width="240px">

この位置にとりつけます。SIM差込口はモジュール内側に向いています。

<img src="https://github.com/akita11/SIM7080module/blob/main/SIM7080mod_solder1.jpg" width="240px">

SIM7080モジュールを基板にあわせてとりつけ（基板の溝にSIMスロットがちょうどはまります）、赤丸の6箇所をはんだ付けします。※アンテナのコネクタがフレームギリギリの位置にきますので、根元に力が加わらないように注意して下さい。


### その2(SIMスロットがモジュール外にある向き）

<img src="https://github.com/akita11/SIM7080module/blob/main/SIM7080mod_usage2a.jpg" width="240px">

この位置に取り付けます。SIM差込口はモジュールの外側に向いています。

<img src="https://github.com/akita11/SIM7080module/blob/main/SIM7080mod_usage2b.jpg" width="240px">

フレームのこの位置をカッター等で加工すれば、モジュールの外側からSIMを抜き差しできます。

<img src="https://github.com/akita11/SIM7080module/blob/main/SIM7080mod_solder2.jpg" width="240px">

SIM7080モジュールの赤丸の端子（6箇所）を基板から1mm程度浮いた状態で、スズメッキ線等ではんだ付けします。（SIM7080モジュールのSIMスロットが基板に密着するように配置します。両面テープ等で固定するとよいでしょう）



## 使い方

SIM7080モジュールとM5Stackコネクタ（Mbusコネクタ）の接続は以下のとおりです。M5Stack側でSerial2等でこれらのIOピンを割り当てて使用して下さい。

- SIM7080のTX（送信）: Mbusの22番（Basic=G13, Core2=G19）
- SIM7080のRX（受信）: Mbusの23番（Basic=G15, Core2=G2）


## Author

Junichi Akita (akita@ifdl.jp, @akita11)
