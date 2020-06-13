geojson:
	ogr2ogr -f GeoJSON city.geojson 市町村等（気象警報等）/市町村等（気象警報等）.shp
	sed -i -e 's/regioncode/code/g' city.geojson
	ogr2ogr -f GeoJSON division.geojson 市町村等をまとめた地域等/市町村等をまとめた地域等.shp
	ogr2ogr -f GeoJSON distlict.geojson 20190125_AreaForecastLocalM_1saibun_GIS/一次細分区域等.shp
	ogr2ogr -f GeoJSON pref.geojson 20190125_AreaForecastLocalM_prefecture_GIS/府県予報区等.shp

mbtiles:
	tippecanoe \
		-o city.mbtiles \
		-l city \
		-z 10 \
		--no-tile-compression \
		-x regionname -x namekana \
		city.geojson
	tippecanoe \
		-o division.mbtiles \
		-l division \
		-z 10 \
		--no-tile-compression \
		division.geojson
	tippecanoe \
		-o distlict.mbtiles \
		-l distlict \
		-z 10 \
		--no-tile-compression \
		distlict.geojson
	tippecanoe \
		-o pref.mbtiles \
		-l pref \
		-z 10 \
		--no-tile-compression \
		pref.geojson

vt:
	tile-join -e . city.mbtiles division.mbtiles distlict.mbtiles pref.mbtiles
