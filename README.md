What is this?
==============

This is documentation for [ngomik.com](http://ngomik.com) API. [Ngomik.com](http://ngomik.com) is a digital comic publishing, especially for Indonesian market. 

**Note**: all documentation in Indonesian, English end here :)

# Cara Penggunaan

## versi 1.0 (recommended)

### Authentication
Mulai versi 1.0, semua API bersifat **private**. Metode yang digunakan adalah Basic HTTP Auth. `app_id` digunakan sebaga username sedangkan `app_secret` digunakan sebagai password.

Untuk mendapatkan `app_id` dan `app_secret`, silakan kontak admin@ngomik.com. 

### Object Property

#### User

    {
        id: "53350",
        username: "uyab",
        email: "bayu.hendra@ngomik.com"
        cash: "1000",
        status: "1",
        created: "2014-02-05 10:49:37",
        modified: "2014-02-05 10:49:37",
        last_activity: "2012-09-12 13:32:51",
        url: "http://api.ngomik.dev/v1/authors/53350",
        permalink: "http://www.ngomik.com/uyab",
        avatar: "http://api.ngomik.dev/img/avatar/53350/100/100/53350.jpg",
        display_name: "Bayu Hendra Winata"
    }



#### Author

    {
        id: "53350",
        username: "uyab",
        email: "bayu.hendra@ngomik.com"
        cash: "1000",
        created: "2014-02-05 10:49:37",
        modified: "2014-02-05 10:49:37",
        last_activity: "2012-09-12 13:32:51",
        url: "http://api.ngomik.dev/v1/authors/53350",
        permalink: "http://www.ngomik.com/uyab",
        avatar: "http://api.ngomik.dev/img/avatar/53350/100/100/53350.jpg",
        display_name: "Bayu Hendra Winata",
        about: "Tukang webcomic",
        cover: "http://api.ngomik.dev/img/user/cover/9983/9983.jpg", // or #FFFFFF
        links: {
            web: "http://4spasi.com",
            facebook: "http://facebook.com/bayu.hendra",
            twitter: false,
            deviantart: false
        }        
    }

#### Series
    
     {
                "id": "8035",
                "slug": "bueuk-ngomik",
                "title": "BUEUK NGOMIK",
                "description": "Sebagai seorang ilustrator di salah satu komunitas dan studio, banyak sekali aktivitas yang tidak/terduga. dan inilah hasil ngupil seharian di meja kerja.",
                "created": "2012-09-03 12:02:26",
                "modified": "2014-01-28 14:53:42",
                "status": "publish",
                "type": "series",
                "quality": "curated",
                "readability": "large",
                "cover_color": null,
                "subscriber_count": "0",
                "url": "http://api.ngomik.dev/v1/series/8035",
                "permalink": "http://www.ngomik.com/comic/bueuk-ngomik/8035",
                "cover": "http://www.ngomik.com/comic/thumb/id/8035/width/640/height/480",
                "thumbnail": "http://www.ngomik.com/comic/thumb/id/8035/width/200/height/300",
                "chapter_count": "8",
                "subscribed": 0,
                "author": <author object>
            }

#### Chapter
    
    {
        "id": "13315",
        "title": "KISAH MALAM MINGGU",
        "slug": "kisah-malam-minggu",
        "created": "2012-09-16 12:48:50",
        "modified": "2012-09-17 07:38:43",
        "published": "2012-09-16 12:54:07",
        "number": "57",
        "status": "publish",
        "url": "http://api.ngomik.dev/v1/chapters/13315",
        "permalink": "http://www.ngomik.com/chapter/13315/kisah-malam-minggu",
        "thumbnail": "http://api.ngomik.dev/img/page/200x300/Y29taWNzLzIwMTIvMDUvMjUvNDA2NTEvNzA2MS8xMzMxNS9wNTA1NWNhYzgyNmNmZjkwODcuanBn/1/gif1.jpg",
        "cover": "http://api.ngomik.dev/img/page/400x600/Y29taWNzLzIwMTIvMDUvMjUvNDA2NTEvNzA2MS8xMzMxNS9wNTA1NWNhYzgyNmNmZjkwODcuanBn/0/gif1.jpg",
        "view_count": "45",
        "comment_count": "3",
        "thumb_count": "6",
        "page_count": "12",
        "synopsis": "Kritik & saran tinggal KOMENT jangan lupa JEMPOLnya yg banyak...!!! {thumb}{thumb}{thumb}{thumb}{thumb}",
        "purchased": 0,
        "price": "0",
        "author": <author object>,
        "series": <series object>,
        "pages": [<array of chpater page object>],
        "prev_chapter": <chapter object>,
        "next_chapter": <chapter object>
    }
    
#### Chapter Page
    {
        "id": "119500",
        "number": "10",
        "url": "http://api.ngomik.dev/img/page/400x600/Y29taWNzLzIwMTIvMDUvMjUvNDA2NTEvNzA2MS8xMzMxNS9wNTA1NWNhZGQ2NGY4MDE4NjYuanBn/0/gif10.jpg"
    }
    
#### Comment

    {
        "id": "292435",
        "chapter_id": "13315",
        "user_id": "50625",
        "content": "jempol melayang mong ",
        "created": "2012-09-16 22:27:09",
        "modified": "2012-09-16 22:27:09",
        "status": "publish",
        "author": <author object>
    }

### Available API

#### Mixed Content
* `GET` [/v1/contents](v1/content.md#index)
* `GET` [/v1/contents/showcase](v1/content.md#showcase)

#### Series
* `GET` [/v1/series](v1/series.md#index)
* `GET` [/v1/series/{id}](v1/series.md#detail)
* `GET` [/v1/series/{id}/comments](v1/series.md#get-comments)

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
* `POST` [/v1/users/create](v1/user.md#me)
* `POST` [/v1/users/{id}/subscribe](v1/user.md#subscribe)
* `POST` [/v1/users/{id}/unsubscribe](v1/user.md#unsubscribe)
* `POST` [/v1/users/buy](v1/user.md#buy)
* `POST` [/v1/users/login](v1/user.md#login)

#### User Collection
* `GET` /v1/users/collections
* `GET` [/v1/users/collections/subscribed](v1/collection.md#subscribed)
* `GET` /v1/users/collections/subscribed/{item_id}
* `GET` /v1/users/collections/subscribed/chapters
* `GET` [/v1/users/collections/purchased](v1/collection.md#purchased)
* `GET` [/v1/users/collections/purchased/{item_id}](v1/collection.md#purchased)

#### Refill Type
* `POST` [/v1/refill_types](v1/refill.md#refill-type)
 
#### Sms
* `POST` [/v1/sms/generate](v1/sms.md#generate)

#### Statistic
* `GET` [/v1/statistic/summary](v1/statistic.md#summary)
* `GET` [/v1/statistic/registration](v1/statistic.md#daily-registration)
* `GET` [/v1/statistic/publication](v1/statistic.md#daily-publication)
* `GET` [/v1/statistic/reader](v1/statistic.md#daily-reader)

#### Subscription
* `POST` [/v1/subscription/list](v1/subscription.md#index)

## versi 0.x (deprecated)

### Authentication
Untuk semua API yang tersedia, bisa diakses di [http://api.ngomik.com](http://api.nogmik.com). API terbagi menjadi 2 jenis, yaitu public dan private. API public bisa diakses oleh siapa saja. API private membutuhkan `app_id` dan `app_secret` untuk mengaksesnya. `app_id` dan `app_secret` ditambahkan sebagai parameter **GET** di url.

Untuk mendapatkan `app_id` dan `app_secret`, silakan kontak admin@ngomik.com. 

