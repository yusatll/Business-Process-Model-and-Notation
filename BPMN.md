# Business-Process-Model-and-Notation  
Şirketlerde yazılım departmanlarında yazılımın nasıl kullanılacağını gösteren flowchartlardır. Türkçe bir kaynak oluşturmak adına paylaşıyorum.
Eksikleri olabilir. Eksik görüdüğünüz yerleri söylerseniz düzeltebilirim.  
Teşekkürler

# BPMN Nedir?  
Business Process Model and Notation kısaltması olan BPMN, şirketlerdeki iş süreçlerini görselleştirmeye yarayan faydalı bir tooldur. Burada amaç işlerin tutarlı ve anlaşılır bir şekilde nasıl yapılacağını, sürecin nasıl işlemesi gerektiğini farklı iş birimlerindeki çalışanlara görsel olarak güzel bir şekilde sunmak ve onlarında bu sürece dahil olmasını sağlamaktır. Bu sayede diğer çalışanlar bu süreç içerisinde neler yapılmasını gerektiğini daha hızlı bir şekilde kavrar.  
  
# Tarihçe  
  
2005 yılında Businss Process Management Initiative (BPMI) tarafından geliştirilmiştir ve Object Management Group (OMG) tarafından sürdürülmektedir. En yaygın kullanılan sürümü 2011 yılında BPMN 2.0 olarak ortaya çıktı. Yeni versiyonunda sub-process (alt işlemler) ile ilgili daha detaylı bilgiler ve kesintiye uğrayan, uğramayan events (olaylar) ile ilgili daha fazla ayrıntı eklendi.
  
  # BPMN’de Bulunan Temel Grafik Unsurlar:
Genellikle soldan sağa olarak çizilen diyagramlar yukarıdan aşağı olarak da çizilebilir. BPMN diyagramı genel anlamda 4 gruba ayrılır: Flow Objects (akış nesneleri), Connecting Objects (Bağlantı nesneleri), Swimlanes / Pool (Havuz) ve Artifacts (Yapay Nesneler).

Her grup kendisine has eylemleri belirtmek için farklı sembollere sahiptir. Şimdi bu nesnelere ve özelliklere bakalım:
  
  **1) Flow Objects:**  
  Flow chart (iş akışı) oluşturmak için birbirine bağlanan nesnelerdir. Bir sürecin davranışını tanımlayan temel unsulardır. Üç çeşit unsur vardır: Event (olay), Activity (aktivite), Gateway (geçit).  

  *-> Event:* Daire sembolü ile gösterilirler. Gerçekleşen bir olayı temsil ederler. Daire içinde olayla ilgili bir bilgi gösterilir.
  
  Mesela daire içinde saat varsa bu tarih veya saati belirtir veya üçgen varsa signal (sinyal) sembolüdür ve farklı işlemler (process) arasında ileşimi sağlar. İçerisinde “ok” varsa bu bir alt process’i gösterir, gibi örnekler verilebilir.

![Event](http://ayusatelli.com/wp-content/uploads/2019/08/event.png "Event")  

  *-> Activity:* Kenarları hafif yuvarlaklaştırılmış dikdörtgen sembolü ile gösterilirler. Bunlar gerçekleştirilen iş süreçleridir (business process). İş ile ilgili kısa bilgi, rapor gibi bilgiler içinde barındırır.
  
  ![Activity](http://ayusatelli.com/wp-content/uploads/2019/08/activ2.png "Activity")

  *-> Gateways:* Paralel kenar başka bir değişle elmas şeklinde gösterilir. Bir activity farklı bir iş süreci akışına geçmesi gerekiyorsa bu geçitler kullanılır. Birkaç farklı çeşidi vardır.
  
  ![Gateways](http://ayusatelli.com/wp-content/uploads/2019/09/gateways.png "Gateways")
  
   *---->  Exclusive:* Akışın durumunu değerlendirir ve bir veya daha fazla yola böler. Akış bu yollardan sadece birine gidebilir. Örneğin yöneticinin onayı ile rapor yazılır, onay vermezse rapor yazılmaz.  
   *---->  Event-based:* Activity’nin gerçekleşip gerçekleşmeme durumunu kontrol eder. Mesela yazılımcının ofise gelinceye kadar mail göndermemek için bekleyip, gelmezse patrona mail gönderebilirsiniz.  
   *---->  Parallel:* Akışı iki veya daha fazla yola böler. Ancak akış bu yollardan hepsine aynı anda devam edebilir.  
   *---->   Inclusive:* Process akışını bir veya daha fazla akışa böler.  
   *---->   Exclusive event-based:* Sonraki olayın gerçekleşmesiyle beraber yeni bir process instance (süreç örneği) başlatır.  
   *---->   Complex:* En karmaşık akışlar için kullanılır. Diğerlerinin uygun olmadığı yerlerde genellikle bu gateway kullanılır.  
   *---->   Parallel event-based:* birden fazla işlemin aynı anda gerçekleşmesini sağlar. Bu işlemler olaya bağlıdır.  

  
  **2) Connecting Objects (Bağlantı nesneleri):**

Akış elemanlarını birbirine bağlar, ilişkilendirir. Üç tane çeşidi vardır: sequence flows, message flows ve associations   
  ![Connecting](http://ayusatelli.com/wp-content/uploads/2019/08/connect.png "Connecting Objects")  
*1. Sequence Flows:* İşlemlerin gerçekleştirildiği sırayı gösterir.  
*2. Message Flows:* Mesajların belirtilen sınırlar arasında akışını gösterir.  
*3. Associations:* Text(metin), arctifact (yapay nesne), veri ve flow objects(akış nesneleri) arasındaki ilişkiyi gösterir.  
  
 **3) Swimlines – Pool:**
 
 Büyük dikdörtgen şeklinde gösterilir. Diyagramın özelliklerini düzenlemek için kullanılır. Nesneleri görsel olarak gruplandırır, flow chart’ı kısımlara ayırarak anlaşılmasını kolaylaştırır diyebiliriz.  
 
  ![Swimlines](http://ayusatelli.com/wp-content/uploads/2019/08/pool.png "Swimlines") Yatay veya dikey şekilde olabilir.  
 
 
 **4) Artifacts (Yapay Nesneler):**  
 Oluşturulan modelle ilgili olan ancak süreçteki unsurlarla ilgili olmayan bilgileri temsil eder. Activity (aktiviteleri) sınıflandırır ve diyagramlardaki processes (işlemler) için daha fazla bilgi gösterilmesini, diyagrama daha fazla bilgi dahil etmek için kullanılır. Üç çeşittir: Data object, group, annotation.  
 
  ![Artifacts](http://ayusatelli.com/wp-content/uploads/2019/08/artifactt.png "Artifacts")
  
   *-> Data Objects:* Process için gerekli verileri gösterir.  
   *-> Group:* Farklı activities (aktiviteleri) gruplandırır.  
   *-> Annotation:* Ek açıklamaların gösterilmesini sağlar.  

 
 # BPMN ÖRNEK
 Aşağıdaki resimde yemek siparişi verirken yaşanan olayları BPMN diyagramında basitçe gösterilmiştir.  
Bu diyagramda gerçekleşen olaylar:  
  01. Müşteri restoranı arar  
  02. Kasiyer telefona cevap verir  
  03. Müşteri restoranın yoğunluğu ile ilgili bilgi alır  
  04. Siparişin gelme süresine göre müşteri karar verir  
  05. Siparişin gelmesi çok uzun sürerse sipariş vermiyor  
  06. Sipariş süresi kısa ise siparişini veriyor  
  07. Kasiyer siparişi alıyor  
  08. Şef siparişi hazırlıyor  
  09. Şef siparişi paketleyip kuryeye veriyor  
  10.Kurye siparişi alıp müşteriye götürüyor  
  11.Müşteri siparişi alıp parasını ödüyor  
  12.Kurye parayı alıp kendi akış diyagramını sonlandırıyor  
  13.Müşteri siparişi yiyip kendi akış diyagramını sonlandırıyor  

![Örnek](http://ayusatelli.com/wp-content/uploads/2019/09/pizza-sipari%C5%9F-1-1024x545.jpg "Örnek")  
  
# Kaynakça  
  
[LucidChart 1](https://www.lucidchart.com/pages/bpmn-bpmn-2.0-tutorial)  
[LucidChart 2](https://www.lucidchart.com/pages/bpmn-symbols-explained)  
  
Online Diyagram Çizmek için:  
[Çizim LucidChart](https://www.lucidchart.com/pages/bpmn-bpmn-2.0-tutorial#section_1)  
ve  
[Draw.io](https://www.draw.io)  
  
Pizza Sipariş Örneği:  
  [Pizza Sipariş](https://www.lucidchart.com/blog/diagrams-for-dummies-a-BPMN-tutorial)
