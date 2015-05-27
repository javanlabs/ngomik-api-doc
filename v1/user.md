### User


#### Create
Mendaftarkan temporary user atau mendapatkan data user jika email sudah terdaftar 

##### url
v1/users/create (POST)

##### parameter
* **email**: valid email address
* **name**: User full name (optional)

##### contoh hasil

    {
        "status": 1,
        "user": {
            "id": "53342",
            "username": "bayuhendra@email.com",
            "email": "bayuhendra@email.com",
            "status": "3",
            "created": "2014-01-21 13:38:06",
            "modified": "2014-01-21 13:38:06",
            "url": "http://api.ngomik.dev/v1/authors/53342",
            "permalink": "http://www.ngomik.com/bayuhendra@email.com",
            "avatar": "http://www.ngomik.com/user/thumb/id/53342",
            "display_name": "bayu hendra winata cak",
            "mode": "existing"            
        }
    }

#### Update
Mengupdate data user

##### url
v1/users/update (POST)

v1/users/{id}/update (POST)

##### parameter
* **name**: user full name
* **avatar**: user avatar file

##### contoh hasil

    {
        "status": 1,
        "user": {
            "id": "53342",
            "username": "bayuhendra@email.com",
            "email": "bayuhendra@email.com",
            "status": "3",
            "created": "2014-01-21 13:38:06",
            "modified": "2014-01-21 13:38:06",
            "url": "http://api.ngomik.dev/v1/authors/53342",
            "permalink": "http://www.ngomik.com/bayuhendra@email.com",
            "avatar": "http://www.ngomik.com/user/thumb/id/53342",
            "display_name": "bayu hendra winata cak"
        }
    }

#### Me
Mendapatkan data pengguna yang sedang login

##### url
v1/users/me (POST)

##### contoh hasil

    {
        "status":1,
        "user":{
            "id":"79933",
            "username":"daniramadani",
            "email":"daniwarrior07@gmail.com",
            "status":"0",
            "created":"2013-11-27 11:56:52",
            "modified":"2015-05-27 14:51:01",
            "cash":"0",
            "followers_count":"0",
            "subscription":{
                "start_date":"2015-05-27 00:00:00",
                "end_date":"2015-05-31 00:00:00",
                "status":1
            }
        }
    }
    
#### Subscribe
User berlangganan suatu konten

##### url
v1/users/subscribe (POST)

v1/users/{id}/subscribe (POST)

##### parameter
* **item_id**: ID item

##### HTTP response code
* `200` OK
* `402` user already subscribe
* `403` active user not found
* `404` series to subscribe not found

##### contoh hasil

    {
        "status": 1,
        "item": {
            "id": "4",
            "slug": "misc-comicstrip",
            "title": "Misc Comicstrip",
            "description": "Comicstrip tidak berkategori",
            "created": "2010-09-02 11:13:34",
            "modified": "2010-11-04 09:54:03",
            "url": "http://localhost/ngomik-api/public/v1/series/4",
            "permalink": "http://www.ngomik.com/comic/misc-comicstrip/4",
            "thumbnail": "http://www.ngomik.com/comic/thumb/id/4/width/200/height/300",
            "chapter_count": "4",
            "author": {
                "id": "8",
                "username": "inoex135",
                "created": "2010-08-29 20:48:45",
                "modified": "2012-09-26 20:26:34",
                "last_activity": "2012-08-04 14:33:42",
                "url": "http://localhost/ngomik-api/public/v1/authors/8",
                "permalink": "http://www.ngomik.com/inoex135",
                "avatar": "http://www.ngomik.com/user/thumb/id/8",
                "display_name": "inoex135"
            }
        }
    }
    
#### Subscribe
User berhenti berlangganan suatu konten

##### url
v1/users/unsubscribe (POST)

v1/users/{id}/unsubscribe (POST)

##### parameter
* **item_id**: ID item

##### HTTP response code
* `200` OK
* `402` user belum berlangganan sebelumnya
* `403` active user not found
* `404` series to unsubscribe not found

##### contoh hasil

    {
        "status": 1,
        "item": {
            "id": "4",
            "slug": "misc-comicstrip",
            "title": "Misc Comicstrip",
            "description": "Comicstrip tidak berkategori",
            "created": "2010-09-02 11:13:34",
            "modified": "2010-11-04 09:54:03",
            "url": "http://localhost/ngomik-api/public/v1/series/4",
            "permalink": "http://www.ngomik.com/comic/misc-comicstrip/4",
            "thumbnail": "http://www.ngomik.com/comic/thumb/id/4/width/200/height/300",
            "chapter_count": "4",
            "author": {
                "id": "8",
                "username": "inoex135",
                "created": "2010-08-29 20:48:45",
                "modified": "2012-09-26 20:26:34",
                "last_activity": "2012-08-04 14:33:42",
                "url": "http://localhost/ngomik-api/public/v1/authors/8",
                "permalink": "http://www.ngomik.com/inoex135",
                "avatar": "http://www.ngomik.com/user/thumb/id/8",
                "display_name": "inoex135"
            }
        }
    }
    
#### Thumbs UP
User memberikan jempol (like) ke suatu chapter

##### url
v1/users/thumbsup (POST)

v1/users/{id}/thumbsup (POST)

##### parameter
* **item_id**: ID item

##### HTTP response code
* `200` OK
* `402` user sudah pernah memberi thumbs up
* `403` active user not found
* `404` series to unsubscribe not found

##### contoh hasil

    {
        "status": 1,
        "item": {
            "id": "1",
            "title": "Alasan Ga Mudik",
            "slug": "alasan-ga-mudik",
            "created": "2010-09-02 09:45:25",
            "modified": "2014-01-14 09:16:45",
            "published": "2010-09-02 02:45:25",
            "number": "1",
            "url": "http://api.ngomik.dev/v1/chapters/1",
            "permalink": "http://www.ngomik.com/chapter/1/alasan-ga-mudik",
            "thumbnail": "http://www.ngomik.com/comicPage/thumb/comic_id/1/page_number/1",
            "page_count": "2",
            "synopsis": "bla bla",
            "author": {
                "id": "8",
                "username": "inoex135",
                "created": "2010-08-29 20:48:45",
                "modified": "2012-09-26 20:26:34",
                "last_activity": "2012-08-04 14:33:42",
                "url": "http://api.ngomik.dev/v1/authors/8",
                "permalink": "http://www.ngomik.com/inoex135",
                "avatar": "http://www.ngomik.com/user/thumb/id/8",
                "display_name": "Wisnu Manupraba"
            },
            "series": {
                "id": "1",
                "slug": "talk-at-office",
                "title": "Talk at Office",
                "description": "Light Joking at the office",
                "created": "2010-09-02 09:44:12",
                "modified": "2010-10-25 08:45:57",
                "type": "series",
                "url": "http://api.ngomik.dev/v1/series/1",
                "permalink": "http://www.ngomik.com/comic/talk-at-office/1",
                "thumbnail": "http://www.ngomik.com/comic/thumb/id/1/width/200/height/300",
                "chapter_count": "3",
                "subscribed": 0,
                "author": {
                    "id": "8",
                    "username": "inoex135",
                    "created": "2010-08-29 20:48:45",
                    "modified": "2012-09-26 20:26:34",
                    "last_activity": "2012-08-04 14:33:42",
                    "url": "http://api.ngomik.dev/v1/authors/8",
                    "permalink": "http://www.ngomik.com/inoex135",
                    "avatar": "http://www.ngomik.com/user/thumb/id/8",
                    "display_name": "Wisnu Manupraba"
                }
            }
        }
    }
    
#### Buy
User membeli konten tertentu

##### url
v1/users/buy (POST)

##### parameter
* **item_id**: ID item

##### HTTP response code
* `200` OK
* `402` Cash tidak cukup untuk membeli
* `406` Item yang dibeli bukan komik berbayar
* `417` User sudah pernah membeli

##### contoh hasil

    {
        "status": 1,
        "item": {
            "id": "417",
            "title": "Jaka Tuang - Mini Series 2",
            "slug": "jaka-tuang-mini-series-2",
            "created": "2010-12-12 18:45:42",
            "modified": "2014-02-14 09:52:13",
            "published": "2010-12-12 18:45:42",
            "number": "2",
            "status": "publish",
            "url": "http://api.ngomik.dev/v1/chapters/417",
            "permalink": "http://www.ngomik.com/chapter/417/jaka-tuang-mini-series-2",
            "thumbnail": "http://api.ngomik.dev/img/page/200x300/Y29taWNzLzIwMTAvMTIvMTAvNzE3LzI3Ni80MTcvNGQwNGI1ZTYwNTAyNC5qcGc=/1/page00.jpg",
            "cover": "http://api.ngomik.dev/img/page/400x600/Y29taWNzLzIwMTAvMTIvMTAvNzE3LzI3Ni80MTcvNGQwNGI1ZTYwNTAyNC5qcGc=/0/page00.jpg",
            "view_count": "2294",
            "comment_count": "73",
            "thumb_count": "42",
            "page_count": "27",
            "synopsis": "Petualangan Jaka Tuang yang membantu seorang bidadari mencari jodoh.\n\nStory & Art: Okky Baskara\nEditing: Mangolang\nPages: 26\nProduction: Bandung, 2009",
            "purchased": 1,
            "price": "1000",
            "author": <object author>,
            "series": <object series>  
        },
        "user": {
            "id": "2",
            "username": "uyab",
            "email": "bayu.hendra@javan.co.id",
            "status": "1",
            "created": "2010-08-23 14:14:44",
            "modified": "2014-02-14 09:52:13",
            "cash": 99000,
            "url": "http://api.ngomik.dev/v1/authors/2",
            "permalink": "http://www.ngomik.com/uyab",
            "avatar": "http://api.ngomik.dev/img/avatar/2/100/100/2.jpg",
            "display_name": "Bayu Hendra Winata"
        }
    }