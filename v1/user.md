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
            "display_name": "bayu hendra winata cak"
        }
    }
    
#### Subscribe
User berlangganan suatu konten

##### url
v1/users/{id}/subscribe (POST)

##### parameter
* **item_id**: ID item

##### contoh hasil

````json
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
````
    
#### Subscribe
User berhenti berlangganan suatu konten

##### url
v1/users/{id}/unsubscribe (POST)

##### parameter
* **item_id**: ID item

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