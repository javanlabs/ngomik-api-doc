### Collection


#### Subscribed
Mendapatkan list of comic yang di-subscribed oleh user

##### url
v1/users/collections/subscribed (mendapatkan koleksi dari auth user)

v1/users/{id}/collections/subscribed (mendapatkan koleksi dari user dengan ID tertentu)

##### parameter
* **page**: untuk menentukan mulai dari urutan keberapa item yang diambil

##### contoh hasil
    
    {
        "total": 1,
        "per_page": 15,
        "current_page": 1,
        "last_page": 1,
        "from": 1,
        "to": 1,
        "data": [
            {
                "id": "8171",
                "slug": "komik-baru",
                "title": "komik baru",
                "description": "test",
                "created": "2013-02-24 07:37:23",
                "modified": "2013-02-24 07:39:32",
                "url": "http://api.ngomik.dev/v1/series/8171",
                "permalink": "http://www.ngomik.com/comic/komik-baru/8171",
                "thumbnail": "http://www.ngomik.com/comic/thumb/id/8171/width/200/height/300",
                "chapter_count": "1",
                "subscribed": 1,
                "author": {
                    "id": "53329",
                    "username": "1338265863",
                    "created": "2013-01-28 02:29:14",
                    "modified": "2013-02-25 17:13:09",
                    "last_activity": "2012-09-28 02:53:27",
                    "url": "http://api.ngomik.dev/v1/authors/53329",
                    "permalink": "http://www.ngomik.com/1338265863",
                    "avatar": "http://www.ngomik.com/user/thumb/id/53329",
                    "display_name": "1338265863"
                }
            }
        ]
    }
    
#### Purchased
Mendapatkan list of comic yang sudah pernah dibeli oleh user

##### url
v1/users/collections/purchased (mendapatkan koleksi dari auth user)

v1/users/{id}/collections/purchased (mendapatkan koleksi dari user dengan ID tertentu)

##### parameter
* **page**: untuk menentukan mulai dari urutan keberapa item yang diambil

##### contoh hasil
    
    {
        "total": 1,
        "per_page": 15,
        "current_page": 1,
        "last_page": 1,
        "from": 1,
        "to": 1,
        "data": [
            {
                "id": "8171",
                "slug": "komik-baru",
                "title": "komik baru",
                "description": "test",
                "created": "2013-02-24 07:37:23",
                "modified": "2013-02-24 07:39:32",
                "url": "http://api.ngomik.dev/v1/series/8171",
                "permalink": "http://www.ngomik.com/comic/komik-baru/8171",
                "thumbnail": "http://www.ngomik.com/comic/thumb/id/8171/width/200/height/300",
                "chapter_count": "1",
                "subscribed": 1,
                "author": {
                    "id": "53329",
                    "username": "1338265863",
                    "created": "2013-01-28 02:29:14",
                    "modified": "2013-02-25 17:13:09",
                    "last_activity": "2012-09-28 02:53:27",
                    "url": "http://api.ngomik.dev/v1/authors/53329",
                    "permalink": "http://www.ngomik.com/1338265863",
                    "avatar": "http://www.ngomik.com/user/thumb/id/53329",
                    "display_name": "1338265863"
                }
            }
        ]
    }