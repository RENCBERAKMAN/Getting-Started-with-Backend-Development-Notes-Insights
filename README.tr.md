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
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=200&section=footer&text=Thanks%20for%20visiting!%20🚀&fontSize=30&fontColor=ffffff" />
</p>

