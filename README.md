What is this?
==============

This is documentation for [ngomik.com](http://ngomik.com) API. [Ngomik.com](http://ngomik.com) is a digital comic publishing, especially for Indonesian market. 

**Note**: all documentation in Indonesian, English end here :)

# Cara Penggunaan

## versi 0.x (deprecated)

### Authentication
Untuk semua API yang tersedia, bisa diakses di [http://api.ngomik.com](http://api.nogmik.com). API terbagi menjadi 2 jenis, yaitu public dan private. API public bisa diakses oleh siapa saja. API private membutuhkan `app_id` dan `app_secret` untuk mengaksesnya. `app_id` dan `app_secret` ditambahkan sebagai parameter **GET** di url.

Untuk mendapatkan `app_id` dan `app_secret`, silakan kontak admin@ngomik.com. 


## versi 1.0 (recommended)

### Authentication
Mulai versi 1.0, semua API bersifat **private**. Metode yang digunakan adalah Basic HTTP Auth. `app_id` digunakan sebaga username sedangkan `app_secret` digunakan sebagai password.

Untuk mendapatkan `app_id` dan `app_secret`, silakan kontak admin@ngomik.com. 

### Available API
#### Mixed Content
* /v1/content/showcase

#### Series
* /v1/series
* /v1/series/{id}

#### Chapters
* /v1/chapters
* /v1/chapters/{id}

#### Authors
* /v1/authors
* /v1/authors/{id}

#### Statistic
* /v1/statistic/summary
* /v1/statistic/registration
* /v1/statistic/publication
* /v1/statistic/reader
