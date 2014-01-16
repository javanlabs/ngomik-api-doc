What is this?
==============

This is documentation for [ngomik.com](http://ngomik.com) API. [Ngomik.com](http://ngomik.com) is a digital comic publishing, especially for Indonesian market. 

**Note**: all documentation in Indonesian, English end here :)

# Cara Penggunaan

## versi 1.0 (recommended)

### Authentication
Mulai versi 1.0, semua API bersifat **private**. Metode yang digunakan adalah Basic HTTP Auth. `app_id` digunakan sebaga username sedangkan `app_secret` digunakan sebagai password.

Untuk mendapatkan `app_id` dan `app_secret`, silakan kontak admin@ngomik.com. 

### Available API
#### Mixed Content
* `GET` [/v1/contents](v1/content.md#index)
* `GET` [/v1/contents/showcase](v1/content.md#showcase)

#### Series
* `GET` [/v1/series](v1/series.md#index)
* `GET` [/v1/series/{id}](v1/series.md#detail)

#### Chapters
* `GET` [/v1/chapters](v1/chapter.md#index)
* `GET` [/v1/chapters/{id}](v1/chapter.md#detail)
* `GET` [/v1/chapters/{id}/comments](v1/chapter.md#get-comments)
* `POST` [/v1/chapters/{id}/comments](v1/chapter.md#post-comments)

#### Authors
* `GET` [/v1/authors](v1/authors.md#index)
* `GET` [/v1/authors/{id}](v1/author.md#detail)

#### Category
* `GET` [/v1/categories](v1/category.md#index)

#### User
* `POST` [/v1/users/create](v1/user.md#index)
* `POST` [/v1/users/{id}/subscribe](v1/user.md#subscribe)
* `POST` [/v1/users/{id}/unsubscribe](v1/user.md#unsubscribe)

#### Sms
* `POST` [/v1/sms/generate](v1/sms.md#generate)

#### Statistic
* `GET` [/v1/statistic/summary](v1/statistic.md#summary)
* `GET` [/v1/statistic/registration](v1/statistic.md#daily-registration)
* `GET` [/v1/statistic/publication](v1/statistic.md#daily-publication)
* `GET` [/v1/statistic/reader](v1/statistic.md#daily-reader)

## versi 0.x (deprecated)

### Authentication
Untuk semua API yang tersedia, bisa diakses di [http://api.ngomik.com](http://api.nogmik.com). API terbagi menjadi 2 jenis, yaitu public dan private. API public bisa diakses oleh siapa saja. API private membutuhkan `app_id` dan `app_secret` untuk mengaksesnya. `app_id` dan `app_secret` ditambahkan sebagai parameter **GET** di url.

Untuk mendapatkan `app_id` dan `app_secret`, silakan kontak admin@ngomik.com. 

