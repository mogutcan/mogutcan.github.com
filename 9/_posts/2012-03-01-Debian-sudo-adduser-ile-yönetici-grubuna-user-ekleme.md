---
layout: post
title: Debian sudo grubuna kullanıcı-yönetici eklemek
---


Debian sistemlerde sudo paketini yükledikten sonra yapılacak iş yönetici 
grubuna kullanıcı eklemektir.Bu işlem yapılmazsa çeşitli programların (19/x gibi)
yüklenmesinde hata ile karşılaşabilirsiniz.

    su

ile root olunur

    gedit /etc/sudoers

açılıp

    root      ALL  = (ALL) ALL

    username  ALL  = (ALL) ALL

satırları eklenir ve kaydedilir.Sistem restart edilir.Burada username
bilgisayarınızda kullandığınız kullanıcı ismidir.

