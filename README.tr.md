<p align="center">
  <img src="https://img.icons8.com/external-flaticons-lineal-color-flat-icons/64/000000/external-coding-web-development-flaticons-lineal-color-flat-icons.png" alt="Coding Icon" />
</p>

## 🔍Backend geliştirici ne iş yapar, frontend’ten farkı nedir?
Backend geliştirici, bir yazılım ya da web uygulamasının görünmeyen kısmını yönetir. Yani kullanıcının tarayıcıda gördüğü arayüzün arkasındaki tüm iş mantığı, veri yönetimi, kullanıcı oturumları, güvenlik, API’ler ve veritabanı işlemleri gibi konular backend tarafında yürütülür.

Frontend, kullanıcının doğrudan etkileşimde olduğu arayüzü inşa ederken; backend geliştirici ise bu arayüzün ihtiyaç duyduğu veriyi sağlamak ve işlemleri gerçekleştirmekle sorumludur.

Örneğin bir kullanıcı bir form gönderdiğinde, bu veriyi alıp veritabanına kaydeden, doğrulayan ve gerektiğinde analiz eden sistem backend tarafında çalışır.

Ben de backend tarafını seçtim çünkü işin mantık ve veri kısmıyla ilgilenmek, karmaşık problemleri çözmek ve sistemin temelini oluşturmak bana çok daha anlamlı ve cazip geliyor.
<hr style="border: 2px solid #4CAF50; margin: 20px 0;">


## 🔍Rest API nedir? Ne işe yarar?
REST API, farklı sistemlerin birbiriyle iletişim kurmasını sağlayan bir yapıdır. Özellikle frontend ve backend’in birbirine veri gönderip alabilmesi için kullanılır.

REST, ‘Representational State Transfer’ anlamına gelir ve HTTP protokolü üzerinden çalışır. API ise bir uygulamanın dış dünya ile iletişim kapısı gibidir.

Örneğin, bir kullanıcı uygulama arayüzünden bir ürün listesi görmek istediğinde, frontend bu isteği backend’e bir REST API aracılığıyla gönderir. Backend bu isteği alır, işleyip veritabanından veriyi çeker ve frontend’e geri gönderir.

✅REST API’ler sayesinde sistemler birbirinden bağımsız çalışabilir, bu da yazılımın ölçeklenmesini ve yönetilmesini kolaylaştırır.
<hr style="border: 2px solid #4CAF50; margin: 20px 0;">

## 🔍HTTP metodları nelerdir? Ne işe yarar?(GET, POST, PUT, DELETE)

“HTTP metodları, bir istemcinin (genellikle frontend’in), sunucuya (backend’e) ne yapmak istediğini belirtmesini sağlar.

En yaygın kullanılan dört temel HTTP metodunu şöyle açıklayabilirim:

GET: Sunucudan veri almak için kullanılır. Örneğin, bir ürün listesini görüntülemek istediğimizde, frontend backend’e GET isteği gönderir.

POST: Sunucuya yeni veri göndermek ve kaydetmek için kullanılır. Mesela bir kayıt formu gönderildiğinde bu işlem POST ile yapılır.

PUT: Var olan veriyi tamamen güncellemek için kullanılır. Örneğin, bir kullanıcının profil bilgilerini güncellerken PUT kullanılır.

DELETE: Belirli bir veriyi sunucudan silmek için kullanılır. Örneğin, bir kullanıcı hesabını silmek için.

✅Bu metodlar sayesinde frontend ve backend arasında düzenli ve anlaşılır bir iletişim olur. REST API’lerde de bu metodları kullanarak farklı işlemleri standart bir şekilde yapabiliyoruz.
<hr style="border: 2px solid #4CAF50; margin: 20px 0;">

## 🔍POST ve PUT arasındaki fark nedir?
POST ve PUT, her ikisi de sunucuya veri göndermek için kullanılır ama amaçları ve kullanıldıkları senaryolar farklıdır.

POST, genellikle yeni bir veri oluşturmak için kullanılır. Örneğin bir kullanıcı kayıt formu gönderirken POST kullanırız. Sunucu yeni bir kullanıcı oluşturur.

PUT ise var olan bir veriyi güncellemek için kullanılır. Örneğin bir kullanıcının e-posta adresini değiştirmek istiyorsak PUT kullanırız.

Bir fark da şudur:

POST her çağrıldığında yeni bir kayıt oluşturabilir (id’si farklı olan yeni nesne gibi),

Ama PUT çağrıldığında belirli bir ID’ye sahip olan veriyi aynı tutarak içeriğini günceller.

✅Kısaca:
→ POST = Oluştur.
→ PUT = Güncelle.
<hr style="border: 2px solid #4CAF50; margin: 20px 0;">

## 🔍Stateless mimari nedir?
Stateless, yani durumsuz mimari, her isteğin (request) birbirinden bağımsız olduğu anlamına gelir. Yani bir istemciden (örneğin bir tarayıcıdan) sunucuya yapılan her istek, sıfırdan yapılır gibi değerlendirilir.

Sunucu, daha önce gelen isteği hatırlamaz. Her istek kendi başına, gerekli tüm bilgileri içerir (örneğin: kimlik doğrulama bilgisi, veri vs.). Böylece sunucu, geçmişe bağlı kalmadan çalışır.
Örnek:
Bir REST API düşün. Her GET veya POST isteğinde sunucuya kim olduğunu ve ne istediğini tekrar tekrar bildirirsin. Sunucu önceki istekte sana cevap vermiş olsa bile, bir sonraki istekte bunu hatırlamaz.

✅ Avantajları:
Sunucu ölçeklenebilir olur (çünkü hafızasında kullanıcı bilgisi tutmaz).

Yük dengeleme (load balancing) kolaylaşır.

Hızlı, basit ve bakımı kolay sistemler kurulur.
<hr style="border: 2px solid #4CAF50; margin: 20px 0;">

## 🔍MVC (Model-View-Controller) Mimarisi Nedir ve Neden Kullanılır?
MVC, üç ana bileşene ayrılmış bir yazılım mimarisidir:

Model (Veri ve İş Mantığı)
Uygulamanın tüm verileri, kuralları ve iş mantığını içerir. Veritabanıyla iletişim, veri işleme ve kurallar bu katmanda yer alır.

View (Görünüm)
Kullanıcının etkileşime geçtiği arayüzdür. Görsel tasarımlar, butonlar, formlar gibi kullanıcıya gösterilen her şey bu katmandadır.

Controller (Kontrolcü)
Kullanıcıdan gelen istekleri işler, uygun Model ile iletişim kurar ve sonucu View’a gönderir. Aslında Model ile View arasındaki bir köprüdür.

-----✅ NEDEN MVC KULLANILIR?-----
1. Kodun Ayrıştırılması (Separation of Concerns)
Her bileşenin kendi sorumluluğu vardır. Böylece kod daha anlaşılır, düzenli ve bakımı kolay hale gelir. Örneğin; görünüm değişirse yalnızca View’ı güncellemek yeterlidir.

2. Test Edilebilirlik Artar
Model ve Controller ayrı olduğundan birimleri test etmek daha kolaydır. Bu, özellikle büyük projelerde otomatik testlerin etkinliği açısından büyük avantaj sağlar.

3. Yeniden Kullanılabilirlik (Reusability)
Aynı veri (Model), farklı görünümlerle (View) birden fazla kez kullanılabilir. Örneğin aynı kullanıcı bilgisi, farklı sayfalarda farklı şekillerde gösterilebilir.

4. Ekipte Paralel Geliştirme Kolaylaşır
Frontend geliştiricileri View üzerinde çalışırken, Backend geliştiricileri Model ve Controller üzerinde çalışabilir. Böylece ekip daha verimli çalışır.

5. Genişlemeye Açık Mimaridir
Uygulama büyüdükçe parçaları büyütmek veya yenilerini eklemek daha kolay hale gelir. Özellikle modüler tasarım isteyen projeler için idealdir.
<hr style="border: 2px solid #4CAF50; margin: 20px 0;">
## 🔍Request ve Response ne demektir?
Request ve Response, web tabanlı sistemlerde istemci (client) ile sunucu (server) arasındaki iletişimi tanımlar. "Request", istemcinin sunucuya gönderdiği istektir. Bu istek, genellikle bir sayfa görüntüleme, veri gönderme veya bilgi alma talebini içerir. Örneğin bir web sitesine giriş yapıldığında, tarayıcı sunucuya bir "GET" isteği göndererek sayfanın içeriğini talep eder.

Sunucu, bu isteği aldıktan sonra işlemi gerçekleştirir ve buna karşılık bir "Response", yani yanıt gönderir. Bu yanıt HTML sayfası, bir JSON verisi, bir hata mesajı ya da işlem sonucunu bildiren başka türde bir içerik olabilir.

Kısaca: Request, istemcinin talebini, Response ise sunucunun bu talebe verdiği cevabı temsil eder. Bu ikili, modern web uygulamalarının temel taşıdır. İletişim genellikle HTTP ya da HTTPS protokolleri üzerinden sağlanır ve her adım belirli kurallarla işler.

Bu yapı sayesinde kullanıcıların tarayıcı üzerinden yaptıkları işlemler sunucu tarafından anlaşılır, işlenir ve karşılık verilir.

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=footer&text=Thanks%20for%20visiting!%20🚀&fontSize=30&fontColor=ffffff" />
</p>

