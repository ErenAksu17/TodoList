<div align="center">

# 📝 TodoList

**Kategori destekli, katmanlı bir ASP.NET Core MVC yapılacaklar uygulaması.**

*A layered ASP.NET Core MVC to-do application with category support.*

![C#](https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=csharp&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core%20MVC-5C2D91?style=flat-square&logo=dotnet&logoColor=white)
![EF Core](https://img.shields.io/badge/Entity%20Framework%20Core-512BD4?style=flat-square&logo=nuget&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![Eğitim projesi](https://img.shields.io/badge/eğitim%20projesi-2023-64748b?style=flat-square)

</div>

> 📌 **Bağlam:** Bu proje 2023'te **Acunmedya Akademi**'deki yazılım geliştirme eğitimim
> sırasında yazıldı. MVC katmanlarını, Entity Framework Core'u ve Razor'u öğrenmek için
> bilinçli olarak sade tutuldu — güncel çalışmalarım için
> [diğer repolarıma](https://github.com/ErenAksu17?tab=repositories) bakabilirsiniz.

---

## 🚀 Özellikler

- ✅ Görev ekleme, güncelleme ve silme
- 📂 Kategori desteği — görevler kategorilere ayrılabilir
- 🔄 Aktif / pasif işaretleme (kalıcı silmeden gizleme)
- 🗂️ Entity Framework Core ile veritabanı yönetimi ve migration
- 🧠 Web / Models / Data olarak ayrılmış temiz MVC yapısı

---

## 🛠️ Kullanılan teknolojiler

| Katman | Teknoloji |
|:--|:--|
| Web çatısı | ASP.NET Core MVC |
| Veri erişimi | Entity Framework Core |
| Veritabanı | SQL Server *(varsayılan)* |
| Görünüm | Razor View Engine |
| Dil | C# |

---

## 📁 Proje yapısı

```text
TodoList/
├── TodoList.Web/            # Ana web uygulaması
│   ├── Controllers/         #   MVC controller dosyaları
│   ├── Views/               #   Razor görünümleri (HTML + C#)
│   ├── wwwroot/             #   Statik dosyalar (CSS, JS)
│   └── appsettings.json     #   Konfigürasyon
├── TodoList.Models/         # Veri modelleri (ToDo, Category ...)
├── TodoList.Data/           # DbContext ve veri erişim katmanı
└── TodoList.sln             # Çözüm dosyası
```

---

## 📦 Kurulum

**Gereksinimler:** .NET SDK ve bir SQL Server örneği (LocalDB yeterlidir).

**1.** Depoyu klonlayın:

```bash
git clone https://github.com/ErenAksu17/TodoList.git
cd TodoList
```

**2.** Projeyi Visual Studio ile açın (`TodoList.sln`).

**3.** `TodoList.Web/appsettings.json` içindeki veritabanı bağlantı dizesini kendi
ortamınıza göre düzenleyin.

**4.** Veritabanını oluşturun — Visual Studio'da **Package Manager Console**:

```powershell
Update-Database
```

Komut satırını tercih ederseniz:

```bash
dotnet ef database update --project TodoList.Data --startup-project TodoList.Web
```

**5.** Uygulamayı çalıştırın ve tarayıcıdan `https://localhost:5001` adresine gidin.

---

## ✍️ Notlar

Kod, okunabilir ve geliştirilebilir olacak şekilde sade tutulmuştur.
Geri bildirimlere her zaman açığım.

---

<div align="center">
<sub>👤 <a href="https://github.com/ErenAksu17">ErenAksu17</a></sub>
</div>
