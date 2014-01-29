### Chapter


#### Index
Mendapatkan list of chapter

##### url
v1/chapters

##### parameter
* **order**: newest, oldest, last-read (only if authUser exist)
* **limit**: berapa banyak item yang ingin diambil
* **page**: untuk menentukan mulai dari urutan keberapa item yang diambil
* **keyword**: untuk mendapatkan chapter yang judulnya mengandung **keyword**

##### contoh hasil
        
    {
        "total": 12632,
        "per_page": 1,
        "current_page": 1,
        "last_page": 12632,
        "from": 1,
        "to": 1,
        "data": [
            {
                "id": "1",
                "title": "Alasan Ga Mudik",
                "slug": "alasan-ga-mudik",
                "created": "2010-09-02 09:45:25",
                "modified": "2012-09-16 18:28:34",
                "published": "2010-09-02 02:45:25",
                "url": "http://localhost/ngomik-api/public/v1/chapters/1",
                "thumbnail": "http://www.ngomik.com/comicPage/thumb/comic_id/1/page_number/1",
                "page_count": "2",
                "synopsis": "bla bla",
                "author": {
                    "id": "8",
                    "username": "inoex135",
                    "created": "2010-08-29 20:48:45",
                    "modified": "2012-09-26 20:26:34",
                    "last_activity": "2012-08-04 14:33:42",
                    "url": "http://localhost/ngomik-api/public/v1/authors/8",
                    "avatar": "http://www.ngomik.com/user/thumb/id/8",
                    "display_name": "inoex135"
                },
                "series": {
                    "id": "1",
                    "slug": "talk-at-office",
                    "title": "Talk at Office",
                    "description": "Light Joking at the office",
                    "created": "2010-09-02 09:44:12",
                    "modified": "2010-10-25 08:45:57",
                    "url": "http://localhost/ngomik-api/public/v1/series/1",
                    "thumbnail": "http://www.ngomik.com/comic/thumb/id/1/width/200/height/300",
                    "chapter_count": "3",
                    "author": {
                        "id": "8",
                        "username": "inoex135",
                        "created": "2010-08-29 20:48:45",
                        "modified": "2012-09-26 20:26:34",
                        "last_activity": "2012-08-04 14:33:42",
                        "url": "http://localhost/ngomik-api/public/v1/authors/8",
                        "avatar": "http://www.ngomik.com/user/thumb/id/8",
                        "display_name": "inoex135"
                    }
                }
            }
        ]
    }
    
#### Detail
Mendapatkan informasi dari suatu chapter

##### url
v1/chapters/{id}

##### parameter
* **id**: ID chapter

##### contoh hasil
        
    {
        "id": "1",
        "title": "Alasan Ga Mudik",
        "slug": "alasan-ga-mudik",
        "created": "2010-09-02 09:45:25",
        "modified": "2012-09-16 18:28:34",
        "published": "2010-09-02 02:45:25",
        "url": "http://localhost/ngomik-api/public/v1/chapters/1",
        "thumbnail": "http://www.ngomik.com/comicPage/thumb/comic_id/1/page_number/1",
        "page_count": "2",
        "synopsis": "bla bla",
        "author": {
            "id": "8",
            "username": "inoex135",
            "created": "2010-08-29 20:48:45",
            "modified": "2012-09-26 20:26:34",
            "last_activity": "2012-08-04 14:33:42",
            "url": "http://localhost/ngomik-api/public/v1/authors/8",
            "avatar": "http://www.ngomik.com/user/thumb/id/8",
            "display_name": "inoex135"
        },
        "series": {
            "id": "1",
            "slug": "talk-at-office",
            "title": "Talk at Office",
            "description": "Light Joking at the office",
            "created": "2010-09-02 09:44:12",
            "modified": "2010-10-25 08:45:57",
            "url": "http://localhost/ngomik-api/public/v1/series/1",
            "thumbnail": "http://www.ngomik.com/comic/thumb/id/1/width/200/height/300",
            "chapter_count": "3",
            "author": {
                "id": "8",
                "username": "inoex135",
                "created": "2010-08-29 20:48:45",
                "modified": "2012-09-26 20:26:34",
                "last_activity": "2012-08-04 14:33:42",
                "url": "http://localhost/ngomik-api/public/v1/authors/8",
                "avatar": "http://www.ngomik.com/user/thumb/id/8",
                "display_name": "inoex135"
            }
        },
        "pages": [
            {
                "id": "1",
                "number": "1",
                "url": "http://www.ngomik.com/comicPage/display/comic_id/1/page_number/1"
            },
            {
                "id": "7",
                "number": "2",
                "url": "http://www.ngomik.com/comicPage/display/comic_id/1/page_number/2"
            }
        ],
        "next_chapter": {
            // chapter object
        },
        "prev_chapter": {
            // chapter object
        }        
    }
    
#### Get Comments
Mendapatkan list of komentar dari suatu chapter

##### url
v1/chapters/{id}/comments (GET)

##### parameter
* **id**: ID chapter
* **page**: page keberapa (untuk paginasi)
* **limit**: berapa banyak komentar yang ingin ditampilkan

##### contoh hasil
        
    {
        "total": 34,
        "per_page": 15,
        "current_page": 3,
        "last_page": 3,
        "from": 31,
        "to": 34,
        "data": [
            {
                "id": "18592",
                "chapter_id": "1",
                "user_id": "1286",
                "content": ":smile::blush::tease:",
                "created": "2011-03-07 19:47:14",
                "modified": "2011-03-07 19:47:14",
                "author": {
                    "id": "1286",
                    "username": "zeal",
                    "created": "2011-01-14 13:37:19",
                    "modified": "2012-09-15 16:55:39",
                    "last_activity": "2011-03-07 12:56:54",
                    "url": "http://api.ngomik.dev/v1/authors/1286",
                    "permalink": "http://www.ngomik.com/zeal",
                    "avatar": "http://www.ngomik.com/user/thumb/id/1286",
                    "display_name": "zeal"
                }
            },
            {
                "id": "22978",
                "chapter_id": "1",
                "user_id": "2354",
                "content": ":good::good::good:",
                "created": "2011-03-24 14:56:18",
                "modified": "2011-03-24 14:56:18",
                "author": {
                    "id": "2354",
                    "username": "pentry",
                    "created": "2011-03-20 23:02:16",
                    "modified": "2012-09-23 01:34:40",
                    "last_activity": "2011-03-25 13:23:07",
                    "url": "http://api.ngomik.dev/v1/authors/2354",
                    "permalink": "http://www.ngomik.com/pentry",
                    "avatar": "http://www.ngomik.com/user/thumb/id/2354",
                    "display_name": "pentry"
                }
            },
            {
                "id": "39873",
                "chapter_id": "1",
                "user_id": "3487",
                "content": ":biggrin::biggrin::good::good: sepp gan",
                "created": "2011-05-27 16:12:52",
                "modified": "2011-05-27 16:12:52",
                "author": {
                    "id": "3487",
                    "username": "Rae_des'vegasz",
                    "created": "2011-05-04 14:58:17",
                    "modified": "2012-05-29 01:19:40",
                    "last_activity": "2012-05-29 01:19:40",
                    "url": "http://api.ngomik.dev/v1/authors/3487",
                    "permalink": "http://www.ngomik.com/Rae_des'vegasz",
                    "avatar": "http://www.ngomik.com/user/thumb/id/3487",
                    "display_name": "Rae_des'vegasz"
                }
            },
            {
                "id": "66383",
                "chapter_id": "1",
                "user_id": "7521",
                "content": "bagusss :signwow:",
                "created": "2011-07-28 17:48:44",
                "modified": "2011-07-28 17:48:44",
                "author": {
                    "id": "7521",
                    "username": "lailas1",
                    "created": "2011-07-25 16:25:39",
                    "modified": "2012-09-16 22:52:43",
                    "last_activity": "2011-10-16 18:08:17",
                    "url": "http://api.ngomik.dev/v1/authors/7521",
                    "permalink": "http://www.ngomik.com/lailas1",
                    "avatar": "http://www.ngomik.com/user/thumb/id/7521",
                    "display_name": "lailas1"
                }
            }
        ]
    }
    
#### Post Comments
Memposting sebuah komentar untuk chapter tertentu

##### url
v1/chapters/{id}/comments (POST)

##### parameter
* **id**: ID chapter
* **user_id**: user ID (optional, jika tidak ada maka akan diisi ID dari auth user)
* **content**: comment message
* **parent_id**: parent comment ID (if this comment is a reply from previous comment)

##### contoh hasil

    {
        "id": "292546",
        "chapter_id": "1",
        "user_id": "2",
        "content": "test",
        "created": "2014-01-21 15:22:14",
        "modified": "2014-01-21 15:22:14",
        "status": "publish",
        "author": {
            "id": "2",
            "username": "uyab",
            "created": "2010-08-23 14:14:44",
            "modified": "2013-12-12 16:42:08",
            "last_activity": "2014-01-07 11:30:46",
            "url": "http://api.ngomik.dev/v1/authors/2",
            "permalink": "http://www.ngomik.com/uyab",
            "avatar": "http://www.ngomik.com/user/thumb/id/2",
            "display_name": "Bayu Hendra Winata"
        }
    }