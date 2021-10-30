#!name=AQI-US
#!desc=iOS 天气使用最精准的空气质量
#!system=ios

[Script]
iOS15美标空气质量 = type=http-response,pattern=^https:\/\/weather-data\.apple\.com\/v2\/weather\/[\w-]+\/-?[0-9]+\.[0-9]+\/-?[0-9]+\.[0-9]+\?,requires-body=true,script-path=https://raw.githubusercontent.com/Vhow123/Vhow-test/master/AQI.js

[MITM]
hostname = %APPEND% weather-data.apple.com

