---
layout: post
title: Cron öğreniyorum!
---



Cron--

Cron ; zamanlanmış görevler demektir.Bilgisayarın belirli bir zamanda bir görevi
otomatik olarak yerine getirmesini istiyorsanız cron tam size göre.

Bir sistem düşünün belirli zamanlarda belirli kullanıcılara mail atmak
zorunda oldugunu farzedelim.Bu görevin gerçekleşeceği tarihi belirterek
Cron Görevleri oluşturabiliriz.


Kullanımı :

    crontab -e     		
-> Edit ; yeni bir cron görevi oluşturmanıza /düzenlemenize yarar.


    crontab -l
-> Mevcut cron görevlerini listeler


cron görevlerinin formatı şu şekildedir :

     * * * * *  /programyolu


 Burada her * bir zaman dilimini ifade eder .
Bu yıldızları sırasıyla açıklayacak olursak

1. Dakika ( 0-59 )

2. Saat (0 -23 )

3. Gün  ( 1- 31 )

4. Ay (1-12)

5. Haftanın günü ( pazar = 0 ,pazartesi = 1 ...)



Cron görevi oluşturabilmek için önce bir komut dosyası hazırlanır.Örneğin
ilk_gorev.sh isminde bir bash-script dosyası oluşturalım ve bu dosyanın içeriği
argüman olarak aldığı e posta adresine mail göndermek olsun.

ilk_gorev.sh scriptini oluşturduktan sonra yapacağımız iş artık bu dosyanın ne
zaman hangi tarihte çalıştırılması gerektiğini söylemek.

Bu iş için

    crontab -e

komutu ile düzenleyeceğimiz görev listesini açıyoruz.( default olarak vim
editöründe açılır) Dosya içine :

    47 22 * * *  /home/mehmet/ilk_gorev.sh 			
-> Bu komut dosyamızın  her gün saat 22.47 de  çalıştırılmasını söyler.

