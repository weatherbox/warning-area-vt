# warning-area-vt
気象庁 細分区域 バイナリベクトルタイル

## generate vector tiles
https://github.com/weatherbox/warning-area
```
tippecanoe -e city -z 10 --no-tile-compression ../warning-area/geojson/city-all.geojson
```

## demo
https://weatherbox.github.io/warning-area/

## data
|        |区域               |url|example|
|:-------|:-----------------|:--|:--|
|pref    |府県予報区          |https://weatherbox.github.io/warning-area-vt/pref/{z}/{x}/{y}.pbf|https://weatherbox.github.io/warning-area-vt/examples/pref.html|
|distlict|一次細分           |https://weatherbox.github.io/warning-area-vt/distlict/{z}/{x}/{y}.pbf|https://weatherbox.github.io/warning-area-vt/examples/distlict.html|
|division|市町村等をまとめた地域|https://weatherbox.github.io/warning-area-vt/division/{z}/{x}/{y}.pbf|https://weatherbox.github.io/warning-area-vt/examples/division.html|
|city    |二次細分           |https://weatherbox.github.io/warning-area-vt/city/{z}/{x}/{y}.pbf|https://weatherbox.github.io/warning-area-vt/examples/city.html|

## ref
- [気象庁 | 気象警報・注意報や天気予報の発表区域](http://www.jma.go.jp/jma/kishou/know/saibun/index.html)
- [気象庁 | 特別警報・警報・注意報や天気予報の発表区域](http://www.jma.go.jp/jma/kishou/know/yougo_hp/shichoson_ichiran.html)

