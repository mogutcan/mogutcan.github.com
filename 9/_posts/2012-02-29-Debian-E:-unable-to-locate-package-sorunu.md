Debian sisteme yeni bir uygulama kurmak istediğinizde 

 apt-get install vim

 E: unable to locate package 

 hatasıyla karşılaşırız . Bunun için bir kaç konfigürasyon yapmak gerek .

 gedit /etc/apt/sources.list

 1-"CD" ile başlayan satırların başına # koy

 2-

 deb http://ftp.sun.ac.za/ftp/debian/ squeeze main non-free contrib
 deb-src http://ftp.sun.ac.za/ftp/debian/ squeeze main non-free contrib

 satırlarını ekle ve kaydet .

 3 - apt-get update 

 güncellemeleri al

 Bunlardan sonra 

  apt-get install sudo 

  komutu başarıyla yüklenecektir.
