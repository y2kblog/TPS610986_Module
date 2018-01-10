# TPS610986 超低消費電力 3.3V出力昇圧モジュール


<img src="/images/ProductImage_Front.jpg" width="200px">




## 概要

超低消費電力の昇圧型DC-DCコンバータ TPS610986 (Texas Instruments Inc.製) を搭載したモジュールです。  
TPS610986の静止電流は約1μA程度（ローパワーモード時）と非常に低いため、バッテリー駆動のアプリケーションに適しています。  
また、TPS610986はロードスイッチ機能が付随しており、MODEピンを利用することでVSUBピンのON/OFFの切り替えとローパワーモード（超低消費電力）/アクティブモード（高過渡応答）の選択が可能です。
これにより、大半の時間はスリープ状態で、定期的にウェイクアップして動作するようなバッテリー駆動のアプリケーションにおいて、常時出力のVMAINピンをマイコンに繋ぎ、VSUBピンをその他のサブシステムに接続することで、スリープ時はローパワーモードでバッテリー寿命を延ばし、ウェイクアップ時はアクティブモードで良好な過渡応答を得ることができます。  
さらに、最大スイッチング電流は350mAであるため、SDカード等の比較的大電流を要するアプリケーションにも使用できます。

<img src="/images/ProductImage_BothSide.jpg" width="400px">

### 仕様
- 入力電圧：0.7V～4.5V (※3.3V以上入力した場合はパススルーとなります)
- 出力電圧：3.3V
- 最大スイッチング電流：350mA (※最大出力電流は入力電圧と効率に依存します)
- ロードスイッチ付
- 効率
  - 88% (入力電圧2V～3.3V、負荷10μA、ローパワーモード時)
  - 93% (入力電圧2V～3.3V、負荷5mA～100mA)
- 基板サイズ：横12.7mm×縦10.0ｍｍ



### 回路図  
<img src="/images/schematic.png" width="500px">

## 販売  
未定
<!--
[スイッチサイエンス委託販売ページ](https://www.switch-science.com/catalog/3493/)  
-->


## 性能評価試験  

### 消費電流量  
<img src="/images/InputVoltage_QuiescentCurrent.png" width="500px">

### 整定時間  

#### VSUBピンの整定時間（負荷：無し）
<img src="/images/SettlingTime_VSUB_NoLoad.jpg" width="400px">

#### VSUBピンの整定時間（負荷：210mA）
<img src="/images/SettlingTime_VSUB_210mA.jpg" width="400px">

#### VMAINピンの整定時間（負荷：無し）
<img src="/images/SettlingTime_VMAIN_NoLoad.jpg" width="400px">

#### VMAINピンの整定時間（負荷：210mA）
<img src="/images/SettlingTime_VMAIN_210mA.jpg" width="400px">


## License
MIT License
