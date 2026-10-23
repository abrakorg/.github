<div align="center">

# Abrak · ABRAK CO
### Akıllı İş Çözümleri Bilişim A.Ş. (Pardazesh-e Rahkar-haye Hooshmand-e Kasb-o-Kar)

**Odoo 19 ve NexERP Tabanlı Kurumsal Bulut ERP Platformu; İran Pazarı ve Teknoloji Odaklı Şirketler İçin Derinlemesine Yerelleştirilmiş, Çok Kiracılı (Multi-Tenant) SaaS Mimarisi**

[**Resmi Web Portalı (abrak.org)**](https://abrak.org) · [**NexERP (zdr.ir)**](https://zdr.ir) · [**Teknik Dokümantasyon**](https://github.com/abrakorg/abrak-docs/tree/main/en)

---

[فارسی](./README.fa.md) • [English](./README.en.md) • [العربية](./README.ar.md) • [Türkçe](./README.tr.md)

</div>

---

## 1. Hakkımızda ve Misyonumuz

**Pardazesh-e Rahkar-haye Hooshmand-e Kasb-o-Kar** (ticari adıyla **Abrak** / **ABRAK CO**), İran'daki üretim, ticaret ve hizmet sektörlerinde faaliyet gösteren modern işletmeler ile özellikle Ar-Ge ve teknoloji odaklı (Danış-bünyan) kurumlar için kurumsal kaynak planlama (ERP) çözümleri tasarlayan, geliştiren ve işleten bir teknoloji şirketidir.

Küresel ölçekteki açık kaynaklı ERP sistemleri, varsayılan olarak Batı muhasebe modelleri, Miladi takvim altyapısı ve uluslararası bankacılık sistemleri üzerine inşa edilmiştir. İran ve çevre bölgesel pazarlarda bu sistemlerin uyarlanması, geçmişte genellikle güvenilir olmayan üçüncü taraf betikleri, yamalar ve yüzeysel çevirilerle yapılmaya çalışılmış; bu durum veri tutarsızlıklarına, performans kayıplarına ve sürüm güncellemelerinde tıkanmalara yol açmıştır.

Abrak bu kronik sorunları **Sıfır Çekirdek Müdahalesi (Zero-Core-Hack)** mühendislik yaklaşımıyla çözmektedir: platform çekirdeği tamamen standart ve el değmemiş olarak korunurken, tüm yerel muhasebe, vergi, takvim ve altyapı entegrasyonları bağımsız, modüler ve sürümler arası uyumlu eklenti (addon) katmanları olarak geliştirilir.

Abrak ekosistemi iki temel kurumsal platformu bünyesinde barındırır:
- **[abrak.org](https://abrak.org)**: **Odoo 19** çekirdeği üzerine kurulu, Kubernetes üzerinde çalışan çok kiracılı (Multi-Tenant SaaS) ve kurumlara özel adanmış dağıtım seçenekleri sunan kurumsal bulut ERP platformu.
- **[zdr.ir](https://zdr.ir)**: Frappe / ERPNext teknoloji yığınını tercih eden işletmeler için özel olarak yapılandırılmış **NexERP** kurumsal yönetim platformu.

---

## 2. Çözdüğümüz Sektörel Sorunlar

İran pazarında faaliyet gösteren kurumsal yapılar, küresel yazılımların standart paketlerinde bulunmayan yasal, mali ve altyapısal gereksinimlerle karşı karşıyadır.

Abrak, işletmelerin bu karmaşık ihtiyaçlarını güvenilir, test edilmiş ve uçtan uca entegre modüllerle karşılamaktadır:

| İran Kurumsal Pazarındaki Temel Zorluklar | Abrak'ın Bütünleşik Mühendislik Çözümü |
|---|---|
| **Yasal Muhasebe ve Defter Standartları:** Küresel hesap planları ve mali tabloların ulusal yasal mevzuatla uyumsuzluğu. | Odoo 19 için yerel mevzuata tam uyumlu çok seviyeli hesap planı, yevmiye ve büyük defterler, dönem/yıl sonu kapanış süreçleri ve yasal mali raporlama altyapısı. |
| **Moadian Elektronik Fatura Sistemi:** Kriptografik imzalama gereklilikleri, değişken veri şemaları ve hatalı bildirim riskleri. | Kriptografik imza yönetimi, şema ve desen doğrulama ile onay öncesi taslak hazırlama modülü (kesinlikle otomatik/kontrolsüz gönderim yapılmaz; yalnızca hazırlık ve doğrulama). |
| **Celali (Hicri Şemsi) Takvimi ve Tarih İşlemleri:** Yüzeysel arayüz maskelerinin veri tabanı sorgularında, faiz/tahakkuk hesaplarında ve iş planlarında sapmalara yol açması. | Doğrudan veri tabanı, ORM, iş mantığı ve raporlama katmanlarına entegre edilmiş, artık yıl hesaplarını kusursuz yöneten ticari **Jalali Pro** takvim motoru. |
| **Haberleşme ve İletişim Altyapısı:** Yerel kurumsal SMS operatörleri, bulut santral (VoIP) ve kargo takip ağlarıyla doğrudan bağlantı eksikliği. | Yerel kurumsal SMS panelleri, bulut santral sağlayıcıları, VoIP operatörleri ve lojistik/dağıtım ağları için önceden yapılandırılmış dayanıklı bağlayıcılar. |
| **Ödeme Geçitleri ve Bankacılık Entegrasyonu:** Uluslararası yazılımların ulusal bankacılık ve ödeme takas ağı (Şaparak) ile iletişim kuramaması. | Yerel bankalar ve yetkili ödeme sağlayıcıları ile güvenli entegrasyon; işlem dönüşünde otomatik muhasebe mutabakatı ve tahsilat kaydı. |
| **Kullanıcı Arayüzü ve Sağdan Sola (RTL) Düzen:** Farsça ve Arapça metinlerde, formlarda, panolarda ve yazdırılabilir PDF faturalarda düzen bozulmaları. | Arayüzün, formların, grafiklerin ve kurumsal PDF şablonlarının temelden iki dilli ve yerel sağdan sola (RTL) tipografi kurallarına göre tasarımı. |
| **Altyapı, Bakım ve Güncelleme Maliyetleri:** Sunucu barındırma, yedekleme, küme yönetimi ve hata ayıklama süreçlerinin şirketlere getirdiği ağır operasyonel yük. | Ölçeklenebilir bulut mimarisi üzerinde, otomatik sağlık denetimi ve olağanüstü durum kurtarma süreçleriyle desteklenen tam yönetimli SaaS hizmeti. |

---

## 3. Yüksek Düzey Mimari ve Teknik Temeller

Abrak platform mimarisi veri gizliliği, operasyonel dayanıklılık, güvenlik ve uzun vadeli sürdürülebilirlik ilkeleri üzerine kurulmuştur:

```
+-----------------------------------------------------------------------------------+
|                            Sunum ve Arayüz Katmanı                                |
|        Kurumsal Web Portalı (abrak.org) · RTL Motoru · Abrak AI ve MCP Araçları   |
+-----------------------------------------------------------------------------------+
                                         │
+-----------------------------------------------------------------------------------+
|                             Uygulama Çekirdek Katmanı                             |
|          Standart Odoo 19 + Modüler Yerelleştirme Ekosistemi (Eklentiler)         |
|     İran Muhasebesi · Jalali Pro · Moadian Taslak Hazırlama · Telekomünikasyon   |
+-----------------------------------------------------------------------------------+
                                         │
+-----------------------------------------------------------------------------------+
|                        Çok Kiracılılık ve İzolasyon Katmanı                       |
|           Veri Tabanı Düzeyinde Tam Kiracı Yalıtımı (Ayrık Şema ve Veri)          |
|                 Sorunsuz Güncellemeler İçin Sıfır Çekirdek Müdahalesi             |
+-----------------------------------------------------------------------------------+
                                         │
+-----------------------------------------------------------------------------------+
|                         Bulut Altyapısı ve Esneklik                               |
|          Kubernetes Üzerinde Konteyner Mimarisi · Çok Kiracılı ve Adanmış Dağıtım |
|         Düzenli Sıcak ve Soğuk Yedekleme · Belgelenmiş Kurtarma Senaryoları       |
+-----------------------------------------------------------------------------------+
```

- **Müdahalesiz Standart Çekirdek:** Platform, Odoo 19'un resmi kaynak kodunu değiştirmeden genişletir; böylece güvenlik yamaları ve sürüm yükseltmeleri kesintisiz uygulanır.
- **Tam Kiracı Yalıtımı (Multi-Tenant Isolation):** Her müşteri organizasyonu tamamen bağımsız bir veri tabanına ve depolama alanına sahiptir. Kiracılar arasında veri sızıntısı mimari düzeyde engellenmiştir.
- **Modern Bulut Orkestrasyonu:** Üretim iş yükleri **Kubernetes** konteyner altyapısı üzerinde çalışır; kesintisiz aşamalı güncellemeler (Zero-Downtime Rolling Updates), otomatik hata onarımı ve dinamik yük dengeleme sağlar. Özel güvenlik gereksinimleri olan kurumlar için adanmış tek kiracılı sunucu kurulumları da desteklenir.
- **Kapsamlı Yedekleme ve Kurtarma (BDR):** Düzenli sıcak ve soğuk yedekleme döngüleri, şifrelenmiş harici depolama ve periyodik olarak test edilen olağanüstü durum kurtarma prosedürleri kesintisiz veri güvenliği sağlar.
- **Kurumsal Yapay Zekâ ve Otomasyon:** Doğal dil işleme arayüzleri, kurumsal asistanlar ve Model Context Protocol (MCP) uç noktalarıyla iş akışlarının kurumsal veri güvenliği çerçevesinde otomatikleştirilmesi.

---

## 4. Kapsanan İşlevsel Alanlar

| İşlevsel Alan | Temel Yetenekler ve Kapsam |
|---|---|
| **Yasal Muhasebe ve Finans** | Standart çok düzeyli hesap planı, resmi yevmiye ve kebir defterleri, mizan, otomatik mali dönem kapanışı, sabit kıymetler ve yasal amortisman takibi. |
| **Moadian E-Fatura Altyapısı** | Dijital imza anahtar yönetimi, benzersiz fatura kimliği üretimi, desen ve şema doğrulaması, onay öncesi hatasız taslak fatura hazırlığı. |
| **Jalali Pro Takvim Motoru** | Veri tabanı sorgularında, iş akışlarında, mali dönemlerde ve tarih seçim bileşenlerinde eksiksiz ve hassas Celali takvimi desteği. |
| **Kurumsal SMS ve Bildirim Sistemi** | Webhook tabanlı bildirimler, sipariş ve fatura durum güncellemeleri, güvenli iki aşamalı doğrulama ve resmi servis hatları entegrasyonu. |
| **Bulut Santral ve VoIP** | Yerel bulut santral sağlayıcıları ile doğrudan entegrasyon, arayan müşteri kartının otomatik gösterimi, çağrı kayıtları ve CRM eşleşmesi. |
| **Ödeme Geçitleri Entegrasyonu** | Çevrim içi ödeme bağlantıları, yetkili banka geçitleri üzerinden tahsilat ve başarılı işlem teyidiyle otomatik cari hesap mutabakatı. |
| **Kalite Yönetim Sistemi (QMS)** | Endüstriyel yemek ve catering sektörü için geliştirilmiş, HACCP ve ISO 22000 standartlarıyla uyumlu özel **Chelopaz** kalite yönetim modülü. |
| **İki Dilli Tipografi ve RTL Düzeni** | Yönetim ve finans terminolojisine uygun profesyonel arayüz dili, standart yazı tipleri ve tüm PDF/tablo belgelerinde hatasız sağdan sola düzen. |

---

## 5. Depo ve Ürün Haritası

ABRAK CO ticari bir kurumsal yazılım sağlayıcısıdır. Fikri mülkiyet haklarını korumak ve kurumsal müşteri verilerinin güvenliğini en üst düzeyde tutmak amacıyla temel yazılım depoları özel (private) olarak yönetilmekte; erişim yetkisi resmi teknik iş birliği ve kurumsal ortaklık anlaşmaları çerçevesinde verilmektedir.

| Depo / Ürün Adı | İşlev ve Kapsam | Erişim Düzeyi |
|---|---|---|
| `abrak-odoo-addons` | Abrak'ın Odoo 19 için geliştirdiği temel kurumsal eklentiler (muhasebe, vergi, iletişim ve SaaS araçları) | Özel depo; iş birliği anlaşması temelinde erişim |
| `abrak-odoo-jalali-pro` | Standart Odoo sürümleriyle uyumlu ticari Celali takvim motoru eklentisi | Herkese açık depo |
| `abrak-calendar-pro` | Odoo 14 ile 19 sürümleri arasındaki kurumsal sürümler için genişletilmiş takvim paketi | Özel depo; iş birliği anlaşması temelinde erişim |
| `abrak-enterprise-governance` | Odoo üzerinde kurumsal yönetişim, süreç denetimi ve yasal uyumluluk modülleri | Özel depo; iş birliği anlaşması temelinde erişim |
| `abrak-odoo-hub-connector-pro` | Harici sistemleri ve üçüncü taraf yazılımları Odoo ile bütünleştiren merkezi bağlantı köprüsü | Özel depo; iş birliği anlaşması temelinde erişim |
| `abrak-connector-php` | Web tabanlı platformları Abrak API'leri ile entegre etmek için geliştirilmiş PHP SDK ve istemci | Özel depo; iş birliği anlaşması temelinde erişim |
| `abrak-connector-python` | Geliştiriciler ve sistem entegratörleri için tasarlanmış Python SDK ve bağlantı kütüphanesi | Özel depo; iş birliği anlaşması temelinde erişim |
| `abrak-landing` | abrak.org platformunun kurumsal web sitesi ve kullanıcı tanıtım portalı | Özel depo; iş birliği anlaşması temelinde erişim |
| `abrak-docs` | Çok dilli resmi ürün dokümantasyonu, kurulum kılavuzları ve teknik bilgi bankası | Herkese açık depo |
| `chelopaz` | Endüstriyel catering ve gıda üretimi için HACCP ve ISO 22000 uyumlu özel Kalite Yönetim Sistemi (QMS) | Özel depo; iş birliği anlaşması temelinde erişim |
| Abrak AI Platformu | Kurumsal yapay zekâ asistanları, RTL/Celali desteği, MCP bağlayıcıları ve otomatik veri işleme hatları | Özel depolar; iş birliği anlaşması temelinde erişim |

> *Güvenlik Notu:* Kurumun iç operasyon, altyapı yönetimi ve sunucu kümeleme bileşenlerine ait depolar güvenlik ve gizlilik politikaları gereğince bu genel listede yer almamakta olup, şirket içi güvenlik protokolleri kapsamında yönetilmektedir.

---

## 6. Mühendislik Standartları ve Güvenlik İlkeleri

Abrak platformunda sistem güvenilirliği ve iş sürekliliği mühendislik süreçlerimizin merkezindedir:

- **Eş Düzey Kod İncelemesi (Peer Code Review):** Hiçbir kod parçası, teknik ekip tarafından mimari ve güvenlik denetiminden geçirilmeden ana depolara birleştirilmez.
- **Otomatik Testler ve Sürekli Entegrasyon (CI):** Tüm eklentiler ve geliştirmeler, canlıya alınmadan önce kapsamlı regresyon ve uyumluluk testlerinden geçirilir.
- **En Az Ayrıcalık İlkesi (Principle of Least Privilege):** Servis hesapları, API anahtarları ve sistem yetkileri yalnızca görevin gerektirdiği asgari düzeyle sınırlandırılmıştır.
- **Önce Yedekleme Dağıtım Protokolü:** Üretim ortamlarındaki tüm sistem değişiklikleri ve sürüm güncellemeleri öncesinde doğrulanmış güncel bir yedek alınması zorunludur.
- **Moadian Yasal Uyum İlkesi (Yalnızca Taslak Hazırlama):** Sistemimiz vergi mevzuatına uygun faturaları hazırlar, doğrular ve taslak olarak düzenler; mali işler yöneticilerinin açık onayı olmaksızın otomatik bildirim gerçekleştirilmez.

---

## 7. İş Birliği ve Kurumsal İletişim

Abrak; teknoloji odaklı işletmeler (Danış-bünyan), sistem entegratörleri ve yazılım geliştirme ekipleriyle kurumsal ortaklıklara açıktır:

- **Teknik İş Birlikleri ve Entegrasyon:** Özel sektörel bağlayıcılar, API tabanlı veri aktarımları ve ortak yazılım çözümleri.
- **Özel Depolara Erişim:** Kurumsal eklentilere ve SDK kaynak kodlarına erişim, imzalanan teknik ortaklık ve gizlilik anlaşmaları kapsamında değerlendirilir.
- **Kurumsal Dağıtım ve Danışmanlık:** Orta ve büyük ölçekli işletmeler için SaaS abonelikleri ve adanmış altyapı kurulumları.

Tüm kurumsal görüşmeler ve iş birliği talepleri için resmi iletişim kanalı:  
👉 [**Resmi Web Portalı: abrak.org**](https://abrak.org)

---

## 8. Sıkça Sorulan Sorular (FAQ)

**Abrak, Odoo'nun çatallanmış (fork) bir sürümü müdür?**  
Hayır. Abrak, Zero-Core-Hack ilkesini titizlikle uygular. Standart Odoo 19 çekirdeği değiştirilmeden korunur; yerelleştirme ve sektörel özellikler modüler eklentiler olarak çalışır. Bu sayede gelecekteki resmi sürümlere geçiş sorunsuz gerçekleşir.

**Abrak yalnızca bulut (SaaS) ortamında mı sunulur, yoksa yerinde kurulum (on-premise) mümkün müdür?**  
Varsayılan modelimiz Kubernetes üzerinde çalışan çok kiracılı SaaS hizmetidir. Ancak yüksek güvenlik veya bağımsız veri barındırma zorunluluğu olan kurumlar için adanmış özel sunucu kurulumları da sağlanmaktadır.

**Abrak, Moadian elektronik fatura sistemine nasıl entegre olur?**  
Platform, vergi dairesi standartlarına uygun fatura verilerinin oluşturulmasını, şematik kontrolünü ve dijital imza altyapısını sağlar. Sistem faturaları taslak olarak hazırlar; mali sorumluluk gereği nihai gönderim işlemi yetkili mali müşavir veya finans yöneticisinin manuel onayı ile tamamlanır.

**abrak.org ile zdr.ir arasındaki ilişki nedir?**  
Her iki platform da aynı kurumsal teknoloji grubuna aittir. abrak.org Odoo 19 tabanlı çözümler sunarken, zdr.ir Frappe/ERPNext mimarisini tercih eden kuruluşlar için NexERP platformunu sağlamaktadır.

**Özel depolara veya geliştirici araçlarına nasıl erişim sağlanabilir?**  
Özel depolara erişim hakkı; onaylı kurumsal müşterilere, entegratör ortaklara ve teknoloji paydaşlarına resmi iş birliği sözleşmeleri ile verilir. Başvurular doğrudan [abrak.org](https://abrak.org) üzerinden iletilebilir.

---

<div align="center">

`Odoo 19` · `ERPNext` · `NexERP` · `SaaS` · `Multi-Tenant` · `Kubernetes` · `Iran Localization` · `Jalali Calendar Pro` · `RTL Native` · `Moadian Invoicing Prep`

<sub>İran'da gururla geliştirildi · Built in Iran</sub>

</div>
