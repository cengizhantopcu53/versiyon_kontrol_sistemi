# Versioning

In our company, we have established a customized versioning format to effectively manage and document the development, prototyping, and production stages of projects undertaken by the R&D department. This guide outlines the specific versioning format and its application in different scenarios.

## Versioning Format

Our versioning format consists of three components: `vX.Y-hZ-fW`.

- `vX.Y`: Represents the production version of the project. The initial version is typically `v1.0`, and subsequent versions are incremented as changes are made or features are added.

- `hZ`: Denotes the hardware prototyping stage. This component is incremented with each new hardware prototype iteration.

- `fW`: Represents the firmware development stage. This component is only included when the firmware is ready for testing or customer release, and it is incremented accordingly.

## Example Scenarios

### New Project and Pre-Production

- Project Start and First Prototyping: `v1.0-h1`
- Second Prototyping: `v1.0-h2`
- Firmware Ready, Customer Release: `v1.0-h2-f1`
- Change in Hardware: `v1.0-h3`
- Firmware Ready, Customer Release: : `v1.0-h3-f2`
- Customer Acceptance Production Release: `v1.0`

### Production with v1.0 
- The customer requests a new feature or development.

### Iterative Development and New Features

- New Features, Change in Hardware: `v1.1-h1`
- Firmware Ready for Testing: `v1.1-h1-f1`
- Additional Testing: `v1.1-h1-f2`
- Customer Acceptance: `v1.1`
- Production Release: `v1.1`

### Production with v1.1

## Guidelines for Usage

1. **Incremental Versioning:**
   - Increment the production version (`vX.Y`) with each change or addition.
   - Increment the hardware prototyping (`hZ`) for each new prototype iteration.
   - Increment the firmware development (`fW`) when firmware is ready for testing or customer release.

2. **Documenting Prototypes:**
   - Include the hardware prototyping (`hZ`) in the version during the prototyping stage to track the evolution of the hardware design.

3. **Firmware Inclusion:**
   - Include the firmware component (`fW`) only when the firmware is ready for testing or customer release.
   - Testing or custumer release include also (`hZ`) part to indicate compatibility of board and firmware.

4. **Customer Release:**
   - When a project is accepted by the customer, release it under the corresponding production version without including the hardware and firmware components.

By adhering to this versioning format, we ensure a clear and organized documentation of our project development process, enabling seamless collaboration between R&D and production teams.

<br>
<br>

# Versiyonlama

Şirketimizde, Ar-Ge bölümü tarafından yürütülen projelerin geliştirme, prototipleme ve üretim aşamalarını etkili bir şekilde yönetmek ve belgelemek için özel bir versiyonlama formatı oluşturduk. Bu rehber, belirli versiyonlama formatını ve farklı senaryolardaki uygulanışını açıklar.

## Versiyonlama Formatı

Versiyonlama formatımız üç bileşenden oluşur: `vX.Y-hZ-fW`.

- `vX.Y`: Projenin üretim versiyonunu temsil eder. İlk versiyon genellikle `v1.0` olup, sonraki versiyonlar değişiklik yapıldıkça veya özellikler ekledikçe artar.

- `hZ`: Donanım prototip aşamasını belirtir. Bu bileşen, her yeni donanım prototip iterasyonu ile arttırılır.

- `fW`: Firmware geliştirme aşamasını temsil eder. Bu bileşen, firmware'in test veya müşteri sürümü için hazır olduğunda sadece dahil edilir ve buna göre arttırılır.

### Yeni Proje ve Üretim Öncesi

- Proje Başlangıcı ve İlk Prototip: `v1.0-h1`
- İkinci Prototipleme: `v1.0-h2`
- Firmware Hazır, Müşteri Sürümü: `v1.0-h2-f1`
- Donanım Değişikliği: `v1.0-h3`
- Firmware Hazır, Müşteri Sürümü: `v1.0-h3-f2`
- Müşteri Kabulü ve Üretim Sürümü: `v1.0`

### Üretimde v1.0 ile Devam
- Müşteri, yeni bir özellik veya geliştirme talep eder.

### İteratif Geliştirme ve Yeni Özellikler

- Yeni Özellikler, Donanım Değişikliği: `v1.1-h1`
- Firmware Test İçin Hazır: `v1.1-h1-f1`
- Ek Testler: `v1.1-h1-f2`
- Müşteri Kabulü: `v1.1`
- Üretim Sürümü: `v1.1`

### Üretimde v1.1 ile Devam

## Kullanım İçin İpuçları

1. **Artan Versiyonlama:**
   - Her değişiklik veya eklemede üretim versiyonunu (`vX.Y`) artırın.
   - Her yeni prototip iterasyonu için donanım prototipleme (`hZ`) artırın.
   - Firmware geliştirme (`fW`), firmware test veya müşteri sürümü için hazır olduğunda artırılır.

2. **Prototipleri Belgeleme:**
   - Donanım prototipleme (`hZ`), prototipleme aşamasında donanım tasarımının evrimini izlemek için versiyona dahil edilir.

3. **Firmware Dahil Etme:**
   - Firmware bileşenini (`fW`), firmware'in test veya müşteri sürümü için hazır olduğunda sadece dahil edin.
   - Test veya müşteri sürümlerine, board ve firmware'in uyumluluğunu belirtmek amacıyla (`hZ`) bileşeni de versiyona dahil edilir.

4. **Müşteri Sürümü:**
   - Bir proje müşteri tarafından kabul edildiğinde, ilgili üretim versiyonu altında sürüm yapın ve donanım ve firmware bileşenlerini içermeyin.

Bu versiyonlama formatına uyarak, projelerimizin geliştirme sürecinin net ve düzenli bir belgelenmesini sağlıyoruz ve Ar-Ge ile üretim ekipleri arasında sorunsuz bir işbirliği sağlıyoruz.
