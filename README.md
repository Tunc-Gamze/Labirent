# Runner Game

## Proje Açıklaması

"Runner Game" bir 3D labirent oyunudur. Oyuncu karakteri, başlangıç noktasından hedefe kadar bir nesneyi götürmeye çalışır. Oyuncu, labirent boyunca karşısına çıkan hedefleri toplar. Oyunun ilerleyen seviyelerinde, labirent duvarlarının hareket etmesi ve kamera açısının düzeltilmesi gibi ek özellikler planlanmıştır.

## İçindekiler

- **playerScript.cs**: Oyuncu karakterinin hareketini ve zıplamasını kontrol eder.
- **cameraScript.cs**: Kamerayı oyuncu karakterini takip edecek şekilde ayarlar.
- **pointScript.cs**: Toplama nesnelerinin, oyuncu tarafından toplandığında yok edilmesini sağlar.

## Kullanılan Teknolojiler

- Unity3D: Oyun motoru.
- C#: Oyun mantığını yazmak için kullanılan programlama dili.

## Oyun Mekanikleri

### Genel Oynanış

- **Sahne:** Oyun sahnesi bir labirentten oluşur.
- **Hedef:** Karakter, başlangıç noktasından hedefe kadar bir nesneyi taşır.
- **Puan Toplama:** Oyuncu, labirent boyunca puan toplamak için belirli hedeflere çarpar.
- **Hareketli Duvarlar:** İlerleyen seviyelerde, labirent duvarlarının hareket etmesi planlanmıştır.

### playerScript.cs

- **Hareket:** Oyuncunun yatay ve dikey hareketleri `Rigidbody` kullanılarak kontrol edilir.
- **Zıplama:** Oyuncu, zemin üzerinde olduğunda `Space` tuşuna basarak zıplayabilir.
- **Çarpışma:** Oyuncu zeminle çarpıştığında `IsGrounded` değişkeni güncellenir.

### cameraScript.cs

- **Kamera Takibi:** Kamera, hedef nesneyi (oyuncu) takip edecek şekilde ayarlanır. Kamera, hedefin arkasında sabit bir mesafede kalır. Kamera açısı, daha iyi bir görünüm için ayarlanabilir.

### pointScript.cs

- **Nesne Toplama:** Oyuncu "point" nesnesine çarptığında, nesne yok edilir ve bir debug mesajı yazdırılır.

## Gelecek Planları

- **Telefon Hareketi:** Oyun, başlangıçta telefon hareketi ile kontrol edilebilecek şekilde tasarlanmıştı. Bu özellik henüz işlevsel değil.
- **Hareketli Labirent Duvarları:** Gelecek seviyelerde, labirent duvarlarının hareket etmesi planlanmıştır.
- **Kamera Açısı:** Kamera açısının iyileştirilmesi gerekmektedir.

## Kurulum ve Çalıştırma

1. Unity Editor'ü açın ve yeni bir proje oluşturun.
2. Yukarıdaki C# dosyalarını projenize ekleyin.
3. Gerekli nesneleri ve komponentleri oluşturun ve script'leri ilgili nesnelere atayın.
4. Oyunu başlatın ve oyuncu karakteri ile etkileşimde bulunarak oyunu test edin.

## Katkıda Bulunanlar

- Gamze Tunç : Proje oluşturucu ve geliştirici.

## Lisans

Bu proje MIT Lisansı altında lisanslanmıştır. Daha fazla bilgi için LICENSE dosyasına bakın.

