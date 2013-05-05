AnyoneInTheHouse?
================

Wireless'a bağlı cihaz olup olmadığını kontrol eden basit bir betik.

Modem'e bağlanıp, istemcilerin listelendiği sayfayı çekiyor. Kaç tane istemci olduğunu sayıp onun sayısını dönüyor. Hata alırsa eksi bir sayı dönüyor. Bağlı istemci olmazsa 0 dönüyor. 

Geliştirmek isteyenler çektiğim html dosyasını şurdan bulabilirler: https://github.com/istanbulhs/AnyoneInTheHouse/blob/master/AnyoneInTheHouseScript/test/data/wlstationlist.cmd

Bağlı Olduğu Kütüphaneler
--------------------------
* Requests (http://docs.python-requests.org/en/latest/)
   
   ```
   pip install requests
   ```
   
Kullanımı
--------------------------
 SimpleHttpServer ile çalışıyor. Ayrıca bir sunucuya ihtiyaç duymuyor.
  
      python -m anyone_in_the_house.py
      
 
Arkasından tarayıcıda: 
 * 
   ```
      http://sunucu/kac-kisi
    ```
   * Bağlı istemci varsa, sayısını dönüyor.
 	* Yoksa 0 dönüyor.
 	* Hata dönerse eksi bir sayı dönüyor.

 * Diğer request'lerde 
 
   * "Kimi aramistiniz?"u dönüyor.
  
 Yapılabilecekler
--------------------------
 * config parametreleri ayri bir dosyaya aktarılabilir
 * Sürekli çalışıp çalışmadığını kontrol eden bir script yazılabilir 
 * bootup'ta betiğin çalışması için linux'ta ne yapılması gerektiği yazılabilir (ve bizim sunucuya da eklenebilir)
 * test yazılabilir
 
 

 


