# Template-Design

#TEMPLATE METHOD TASARIM DESENI
Desenin Amacı: Bir işlemde yapılması gereken bazı adımları alt sınıflara bırakarak bir
algoritma taslağı oluşturmayı sağlar. Alt sınıflar algoritmanın genel yapısını
değiştirmeden algoritmadaki belli başlı adımları yeniden tanımlar.

## Uygulanabilirlik: Aşağıdaki durumlarda bu deseni kullanın:
- Değişmeyen davranışlar bir kere tanımlanacaksa ve değişen
davranışlar alt sınıflara bırakılacaksa.
- Altsınıfların genişlemesini kontrollü bir şekilde yapmak
istiyorsanız.
- Bunu da Template metodun içinde “hook” olarak adlandırılan belli
noktalarda çağrılan işlemler tanımlayarak yapabilirsiniz.
## Katılımcılar:
- AbstractClass (SoyutSinif, Uygulama):Soyut temel işlemlerin,
algoritma şablonunu oluşturacak template method’un tanımlandığı
sınıf. Template method bu sınıf içinde tanımlı temel işlemleri ve
diğer işlemleri çağırır.
- ConcreteClass(SomutSinif,SomutUygulama): Alt sınıflara özel
temel işlemleri gerçekleştirir.
## Sonuçlar:
- Kodun yeniden kullanılabilirliğini artırır.
- Kontrollü bir yapı oluşturmayı sağlar. Hollywood Prensibi de denilen
‘Bizi arama, biz seni ararız(Don’t call us, we’ll call you)’ prensibini
uygular. Bu prensip üst sınıfın alt sınıfın metodlarını nasıl çağıracağını,
tam tersinin olamayacağını belirtir.
## Kullanım Alanları:
- java.util.AbstractList
- Servlet doGet and doPost metodlari
- Struts framework’de Action sınıfı
- Spring framework’de veri erişim sınıfları
