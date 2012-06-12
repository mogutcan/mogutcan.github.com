---
layout: post
title: Linux için JAVA SANAL MAKİNESİ kurulumu
---


Linux işletim sistemine Java Sanal Makinesi (JVM) nasıl kurulur

Adım 1:

 [Oracle'ın resmi sitesinden](http://www.oracle.com/technetwork/java/javase/downloads/index.html)

Java Development Kit (JDK) en son sürümü .tar.gz uzantısı
secilerek indirilir.



Adım 2:
  
   İndirilen JDK dosyasını hangi dizin altında extract ederseniz
   JVM oraya kurulmuş olur.
   Bu anlatımda kurulumu /opt/ dizinine yaptığınızı varsayıyorum.

 

       tar zxvf jdk-7u<version>-linux-x64.tar.gz

şeklinde sıkıştırılmış dosya açılır.

Adım 3:

      
  Sisteme JVM kurulumunu tanıtmak için sistem path konfigürasyonu
       
       echo $PATH
 
PATH çıktısı kopyalanır.

       vi ~/.bashrc

içine 
 
       PATH=<kopyalanan_cikti>:/opt/jdk1.7.0_04/bin  
eklenir.

Son olarak PATH güncellemesi yapılır.

      source ~/.bashrc

Kurulumunuzun doğruluğunu

      java -version

çıktısına bakarak anlayabilirsiniz.


