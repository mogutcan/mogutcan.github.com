---
layout: post
title: Vim kullanımı
---

Vim linux üzerinde bulunan metin editörlerinden birisidir.Kullanımı karmaşık gibi görünsede kullanıldıkça vazgeçilmez bir hale geliyor.
Vim etkili kod/yazı yazmayı sağlarken hızlanmayı da sağlıyor.

Komutlar :


    vim deneme.txt 	         	-> deneme.txt adında bir dosya oluşturur.

    i                            	-> vim de yazı yazma moduna geçer(insert)

    ESC 				-> ESC tuşu ile komut verme moduna geçilir.Yani komut vermek
       	    	  			   için her defasında esc tusuna basılmalı.

    :q 				        -> Çıkmak için kullanılır.Kaydetmeden çıkılırsa hata verir.

    :wq 				-> Yaz ve çık

    h 				        -> Metin üzerinde sola gider

    l 	       			        -> Sağa gider

    k 					-> Yukarı

    j 					-> Asağı

Not:Yön tuşları yerine h-l-j-k kullanımı hızlanmayı sağlar.

    fm 					-> "Sadece" bulundugu satırda ileriye doğru  'm' araması yapar.

    Fa 					-> "Sadece" bulundugu satırda geriye doğru  'a' araması yapar.

    0 					-> Satır başına git

    $ 					-> Satır sonuna git

2$ 		-> Bir alttaki satırın sonuna git

5$ 	        -> 4 alttaki satırın sonuna git

33w 		-> 33 kelime ileri git

14b 		-> 14 kelime geri git

G 		-> Dosyanın son satırına git

1G 		-> Dosyanın ilk satırına git

24G 		-> Dosyanın 24.satırına git

33w 		-> 33 kelime ileri git

14b 		-> 14 kelime geri git

G 		-> Dosyanın son satırına git

1G 		-> Dosyanın ilk satırına git

24G 		-> Dosyanın 24.satırına git

33w 		-> 33 kelime ileri git

14b 		-> 14 kelime geri git

G 		-> Dosyanın son satırına git

1G 		-> Dosyanın ilk satırına git

24G 		-> Dosyanın 24.satırına git

33w 		-> 33 kelime ileri git

14b 		-> 14 kelime geri git

G 		-> Dosyanın son satırına git

1G 		-> Dosyanın ilk satırına git

24G 		-> Dosyanın 24.satırına git

:set number 	-> Ekranın soluna satır numaraları ekler!
:set nonumber 	-> Satır numaralarını kaldırır.

/linux 		-> İleriye doğru giderek Linux kelimesini arar.

:set hlsearch 	-> Aranan kelimeleri renklendirir.
:set nohlsearch -> hlsearch özelliğini kapatır.

yy 		-> Bulundugu Satırı kopyalar
3y 		-> 3 satırı kopyalar

. 		-> Kopyalanan satırı yapıştırır

G 		-> Dosya sonuna git

~ 		-> İmlecin bulundugu yerdeki harfi kücük/büyük harfle değiştir
4~ 		-> önündeki 4 karakteri kücük/büyük harfe dönüştür.

:split 	        -> Ekranı pencerelere böl

vim -O a.c b.c  -> Dikey pencerelerde 2 dosya açar.

vim -o a.c b.c  -> Yatay pencerelerde 2 dosya açar.(a.c ve b.c)

CTRL+W 		-> Yatay ve dikey pencereler arası geçiş.

v 		-> Visual mod
		-> Bu modda fare ile hareket ettirilen satırlar renklenir.

> 		-> Bulundugu satırı shift genişliği kadar kaydırır(Visual modda)

:syntax on 	-> Tanınmayan dosya türlerinde metni renklendirir

:set shiftwidth=4 	-> Tab boşluğunu ayarlar

:mkvimrc dosyaismi 	-> set vb yapılan ayarların saklanmasını sağlar.

:source dosyaismi 	-> kaydedilen ayarları çağırır.

						





