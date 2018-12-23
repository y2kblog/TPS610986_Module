# TPS610986 超低消費電力 3.3V出力昇圧モジュール

<!--
<img src="/images/ProductImage_Front.jpg" width="200px">
-->
<img src="/images/ProductImage_BothSide.jpg" width="300px">


## 概要

超低消費電力の昇圧型DC-DCコンバータ TPS610986 (Texas Instruments Inc.製) を搭載したモジュールです。  
TPS610986の**静止電流は約1μA程度**（ローパワーモード時）と非常に低く、また**0.7Vから動作**するため、コイン電池1個、もしくはアルカリ／ニカド／ニッケル水素乾電池1～2本で駆動するアプリケーションに適しています。  
さらに、TPS610986は**ロードスイッチ機能付き**であり、MODEピンを利用することでVSUBピンのON/OFFの切り替えとローパワーモード（超低静止電流）／アクティブモード（高過渡応答）の選択が可能です。  
これにより、定期的にウェイクアップして動作し、それ以外の大半の時間はスリープするようなバッテリー駆動のアプリケーションにおいて、常時出力のVMAINピンをマイコン（MCU）に繋ぎ、VSUBピンをその他のサブシステム（センサ、GPS、無線モジュール、SDカード等）に接続すると、スリープ時はローパワーモードでマイコンのみに電力を供給することでバッテリー寿命を延ばし、動作時はアクティブモードでサブシステムにも高過渡応答の安定的な電力を供給する、といったことが可能です。  
<!--
TPS610986の静止電流は約1μA程度（ローパワーモード時）と非常に低いため、バッテリー駆動のアプリケーションに適しています。  
-->
<!--
スリープ時はローパワーモードでマイコンのみに電力を供給することでバッテリー寿命を延ばし、ウェイクアップ時はアクティブモードで良好な過渡応答を得ることができます。  
また、最大スイッチング電流は350mAであるため、SDカード等の比較的大電流を要するアプリケーションにも使用できます。
-->


<img src="/images/LowPowerSystem.jpg" width="500px">


### 仕様
- 入力電圧：0.7V～4.5V (※3.3V以上入力した場合はパススルーとなります)
- 出力電圧：3.3V (低負荷のバーストモード時：3.4V)
- 最大スイッチング電流：350mA (※最大出力電流は入力電圧と効率に依存します)
- ロードスイッチ付
- 効率
  - 88% (入力電圧2V～3.3V、負荷10μA、ローパワーモード時)
  - 93% (入力電圧2V～3.3V、負荷5mA～100mA)
- 基板サイズ：横12.7mm×縦10.0ｍｍ

## 販売  
[スイッチサイエンス委託販売ページ](https://www.switch-science.com/catalog/3659/)  
※大量注文や在庫に関する問い合わせは[こちら](mailto:info.y2kb@gmail.com)までご連絡ください。  

### 回路図  
<img src="/images/schematic.png" width="500px">

### 寸法
<img src="/images/TPS610986_Module_PCBsize.png" width="200px">

## 性能評価  

### 静止電流  
<img src="/images/InputVoltage_QuiescentCurrent.jpg" width="500px">

### 整定時間  

#### VSUBピンの整定時間（負荷：無し）：約800μs
<img src="/images/SettlingTime_VSUB_NoLoad.jpg" width="400px">

#### VSUBピンの整定時間（負荷：210mA）：約760μs
<img src="/images/SettlingTime_VSUB_210mA.jpg" width="400px">

#### VMAINピンの整定時間（負荷：無し）：約580μs
<img src="/images/SettlingTime_VMAIN_NoLoad.jpg" width="400px">

#### VMAINピンの整定時間（負荷：210mA）：約1500μs
<img src="/images/SettlingTime_VMAIN_210mA.jpg" width="400px">

## データシート  
[TPS610986データシート(英語)](http://www.ti.com/lit/ds/symlink/tps610986.pdf)

## License
MIT License
