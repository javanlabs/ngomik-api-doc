### Chapter


#### Index
Mendapatkan list of chapter

##### url
v1/chapters

##### parameter
* **order**: newest, oldest
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
        ]
    }