# Fullstack Blog Uygulaması (Laravel + React)

Bu proje, Laravel ile geliştirilmiş bir RESTful API ve React frontend'inden oluşan tam işlevli bir blog uygulamasıdır. Uygulama, kullanıcıların kayıt olup giriş yapabileceği, post paylaşabileceği, yorum yazabileceği ve gönderileri beğenebileceği temel sosyal medya benzeri özellikler sunar.

## Özellikler

- Kullanıcı kayıt ve giriş sistemi (JWT - Laravel Sanctum)
- Post oluşturma, listeleme ve silme (sadece sahibi tarafından silinebilir)
- Postlara yorum yapma ve yorum silme (sadece yorumu yapan kullanıcı tarafından)
- Beğeni sistemi (kullanıcı başına tek beğeni, toggle sistemi)
- Post detay sayfasında yorumlar ve beğeni durumu gösterimi
- Auth middleware ile güvenli API erişimi
- React frontend ile dinamik kullanıcı arayüzü
- SQLite veritabanı ile kolay geliştirme ortamı

## Kullanılan Teknolojiler

### Backend

- Laravel 10
- Laravel Sanctum
- SQLite

### Frontend

- React (create-react-app)
- Tailwind CSS
- Axios
- React Router DOM

## Demo Kullanıcı Bilgileri

Proje arayüzünü test etmek için aşağıdaki demo kullanıcı bilgilerini kullanabilirsiniz:

E-posta: omercylnn@hotmail.com
Şifre: 123456


## Kurulum

### 1. Repository'yi klonla

```bash
git clone https://github.com/omerrcylnn/blog-app.git
cd blog-app

 Backend Kurulumu

cd backend
composer install
cp .env.example .env
php artisan key:generate

# SQLite dosyası oluştur
touch database/database.sqlite

# .env dosyasında DB_CONNECTION=sqlite olarak ayarla
php artisan migrate --seed
php artisan serve

Backend URL: http://localhost:8000/api

3. Frontend Kurulumu
cd ../frontend
npm install
npm start

Frontend URL: http://localhost:3000

Klasör Yapısı

blog-app/
├── backend/      # Laravel API (Sanctum, Posts, Comments, Likes)
├── frontend/     # React uygulaması (Auth, Post, Yorum, Beğeni)
└── README.md



Gelecekte Planlanan Geliştirmeler
Yorum düzenleme özelliği

Post ve kullanıcı arama / filtreleme

Responsive tasarım geliştirmeleri

Canlı demo yayını (Render, Netlify, Vercel vb.)

Basit rol yetkilendirme sistemi

Test altyapısı (Feature / Unit tests)

Geliştirici
Güner Ömer Ceylan
https://github.com/omerrcylnn
