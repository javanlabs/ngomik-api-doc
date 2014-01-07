### User


#### Create
Mendaftarkan temporary user atau mendapatkan data user jika email sudah terdaftar 

##### url
v1/users/create (POST)

##### parameter
* **email**: valid email address

##### contoh hasil

    {
        "status": 1,
        "user": {
            "id": "53340",
            "username": "bayuhendra@javan.com",
            "email": "bayuhendra@javan.com",
            "status": "3",
            "created": "2014-01-07 10:16:44",
            "modified": "2014-01-07 10:16:44"
        }
    }
    
#### Subscribe
User berlangganan suatu konten

##### url
v1/users/{id}/subscribe (POST)

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