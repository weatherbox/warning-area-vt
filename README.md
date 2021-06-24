# warning-area-vt
気象庁 細分区域 ベクトルタイル

## demo
https://weatherbox.github.io/warning-area/

## data
- url `https://weatherbox.github.io/warning-area-vt/pref/{z}/{x}/{y}.pbf`
- example https://weatherbox.github.io/warning-area-vt/v2/example.html

|layer   |区域                |Property|
|:-------|:-------------------|:-------|
|pref    |府県予報区          |code,name|
|distlict|一次細分            |code,name|
|division|市町村等をまとめた地域|code,name|
|city    |二次細分           |code,name|

### 出典
気象庁 予報区等GISデータ「市町村等（気象警報等） 」、「市町村等をまとめた地域等」、「一次細分区域等」、「府県予報区等 」を加工して作成
http://www.data.jma.go.jp/developer/gis.html

### 更新履歴
- 2020年5月29日　栃木県日光市の予報区分割


## ref
- [気象庁 | 気象警報・注意報や天気予報の発表区域](http://www.jma.go.jp/jma/kishou/know/saibun/index.html)
- [気象庁 | 特別警報・警報・注意報や天気予報の発表区域](http://www.jma.go.jp/jma/kishou/know/yougo_hp/shichoson_ichiran.html)

