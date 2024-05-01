# MyChat

## Açıklama 
Agora Web SDK kullanılarak bir Django arka ucu ile Grup video görüşmesi uygulaması.

## Bu kaynak kodunu nasıl kullanabilirim

#### 1 - Depoyu klonla
```
git clone https://github.com/divanov11/mychat
```

#### 2 - Gereksinimleri yükle
```
cd mychat
pip install -r requirements.txt
```

#### 3 - Agora kimlik bilgilerini güncelle
Bu projeyi kullanmak için, `views.py` ve `streams.js` dosyalarında agora kimlik bilgilerini değiştirmeniz gerekecektir.

Agora.io adresinde bir hesap oluşturun ve bir `uygulama` oluşturun. Uygulamanızı oluşturduktan sonra, `appid` ve `appCertificate`'yi kopyalayarak `views.py` ve `streams.js` dosyalarını güncellemeniz gerekecektir. Uygulamanız hakkında nereden bilgi alabileceğiniz hakkında sorularınız varsa, bu bağlantıyı referans almanızı öneririm `https://youtu.be/HX6AM_1-jNM?t=88`

###### views.py
```
def getToken(request):
    appId = "UYGULAMA KİMLİK NUMARASI"
    appCertificate = "UYGULAMA SERTİFİKASI"
    ......
```

###### streams.js
```
....
const APP_ID = 'UYGULAMA KİMLİK NUMARASI'
....
```

#### 4 - Sunucuyu Başlat
```
python manage.py runserver
```


