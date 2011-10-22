$w = new googleWeather();
$w->enable_cache = 1;
$w->cache_path = '/var/www/mysite.com/cache';

$ar_data = $w->get_weather_data(10027);

print_r($ar_data);

echo $ar_data['forecast'][0]['day_of_week'];