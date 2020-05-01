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
  
  1) Flow Objects: Flow chart (iş akışı) oluşturmak için birbirine bağlanan nesnelerdir. Bir sürecin davranışını tanımlayan temel unsulardır. Üç çeşit unsur vardır: Event (olay), Activity (aktivite), Gateway (geçit).  

  -> Event: Daire sembolü ile gösterilirler. Gerçekleşen bir olayı temsil ederler. Daire içinde olayla ilgili bir bilgi gösterilir.
  
  Mesela daire içinde saat varsa bu tarih veya saati belirtir veya üçgen varsa signal (sinyal) sembolüdür ve farklı işlemler (process) arasında ileşimi sağlar. İçerisinde “ok” varsa bu bir alt process’i gösterir, gibi örnekler verilebilir.

![Event](http://ayusatelli.com/wp-content/uploads/2019/08/event.png)
