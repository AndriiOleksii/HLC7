# HLC7
Highload Course. Ex 7

1. В папці WeatherAPI знаходиться сервер на net core
2. docker-compose.yml - піднімає сервер та ngnix
3. nginx.conf -  налаштування nginx з кешом
 а) proxy_cache_min_uses 2; - відповідає за к-сть викликів до кешування
 б) proxy_cache_bypass $http_secret_header; - при прокидуванні [{"key":"secret-header","value":"True","description":"","type":"text","enabled":true}] в хідері очищується кеш конкретного ресурсу
