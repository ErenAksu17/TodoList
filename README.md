# 📝 TodoList Uygulaması

Bu proje, ASP.NET Core MVC mimarisi kullanılarak geliştirilmiş basit ve işlevsel bir yapılacaklar listesi (ToDo) uygulamasıdır. Kullanıcılar görevlerini oluşturabilir, kategorilere ayırabilir, silebilir ve pasif hale getirebilir.

## 🚀 Özellikler

- ✅ Görev ekleme, silme ve güncelleme
- 📂 Kategori desteği
- 🔄 Görevleri aktif/pasif olarak işaretleme
- 🗂 Entity Framework Core ile veritabanı yönetimi
- 🧠 Temiz MVC yapısı

## 🛠️ Kullanılan Teknolojiler

- ASP.NET Core MVC
- Entity Framework Core
- SQL Server (Varsayılan)
- Razor View Engine
- C#

## 📁 Proje Yapısı

```
TodoList/
│
├── TodoList.Web/           → Ana web uygulaması
│   ├── Controllers/        → MVC Controller dosyaları
│   ├── Views/              → Razor View dosyaları (HTML + C#)
│   ├── wwwroot/            → Statik dosyalar (CSS, JS)
│   └── appsettings.json    → Konfigürasyon
│
├── TodoList.Models/        → Veri modelleri (ToDo, Category vs.)
├── TodoList.Data/          → DbContext ve veri erişim katmanı
└── TodoList.sln            → Çözüm dosyası
```

## 📦 Kurulum

1. Bu repoyu klonlayın:
   ```bash
   git clone https://github.com/ErenAksu17/TodoList.git
   
2. Projeyi Visual Studio ile açın.

3. appsettings.json dosyası üzerinden veritabanı bağlantı ayarlarını yapılandırın.

4. Migration ve database oluşturmak için:
   ```bash
   Update-Database

6. Uygulamayı çalıştırın ve tarayıcıdan https://localhost:5001 adresine gidin.

## ✍️ Notlar
Proje, Acunmedya Akademi'deki yazılım geliştirme eğitimim sürecinde geliştirilmiştir.

Kod sade ve geliştirilebilir olacak şekilde tasarlanmıştır.

Geri bildirimlere her zaman açığım!
