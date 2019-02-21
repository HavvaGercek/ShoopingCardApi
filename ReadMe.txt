Sepete �r�n Ekleme API

Uygulamay� ba�latmdan �nce Redis ayarlar�n�n yap�lmas� gerekmektedir.


Startup/ConfigureServices i�erisinde options.Configuration k�sm� g�ncelenmeli ve redis server �al���r halde olmal�d�r.

services.AddDistributedRedisCache(options =>
  {
      options.InstanceName = "RedisNetCore";
      options.Configuration = "localhost: 6379"; //Your Redis connection port
  });


Ap� Kullan�m� i�in:  http://localhost:15350/swagger/index.html 
