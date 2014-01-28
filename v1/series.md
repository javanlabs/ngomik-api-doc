### Series


#### Index
Mendapatkan list of series

##### url
v1/series

##### parameter
* **type**: 'all', 'series', 'oneshot', 'strip' (default 'all')
* **order**: newest, oldest
* **limit**: berapa banyak item yang ingin diambil
* **page**: untuk menentukan mulai dari urutan keberapa item yang diambil
* **keyword**: untuk mendapatkan series yang judulnya mengandung **keyword**
* **google_token**: identifier user jika mengakses dari android device

##### contoh hasil

    {
        "status": 1,
        "total": 1250,
        "per_page": 2,
        "current_page": 1,
        "last_page": 625,
        "from": 1,
        "to": 2,
        "data": [
            {
                "id": "562",
                "slug": "what-the",
                "title": "What The",
                "description": "Komik 1 halaman... iseng2 bikin untuk mengisi waktu luang...",
                "created": "2011-02-07 22:21:15",
                "modified": "2014-01-28 14:41:05",
                "status": "publish",
                "type": "series",
                "cover_color": "#dddddd",
                "url": "http://api.ngomik.dev/v1/series/562",
                "permalink": "http://www.ngomik.com/comic/what-the/562",
                "thumbnail": "http://www.ngomik.com/comic/thumb/id/562/width/200/height/300",
                "chapter_count": "2",
                "subscribed": 0,
                "author": {
                    "id": "1454",
                    "username": "adisty_tir.sia_atreides_ii",
                    "created": "2011-01-26 20:37:08",
                    "modified": "2012-09-28 01:20:36",
                    "last_activity": "2011-06-09 18:31:31",
                    "url": "http://api.ngomik.dev/v1/authors/1454",
                    "permalink": "http://www.ngomik.com/adisty_tir.sia_atreides_ii",
                    "avatar": "http://api.ngomik.dev/img/avatar/1454/100/100/1454.jpg",
                    "display_name": "Adisty Solihah"
                }
            },
            {
                "id": "563",
                "slug": "battleloid",
                "title": "BattleLoid",
                "description": "bercerita tentang para Sulmerian, manusia dengan kemampuan khusus sejak lahir. tapi kini mereka menjadi langka akibat pembantaian para Sulmerian 3 tahun yang lalu. dan kami, para ilmuwan dari Mundock Research Facilities, memiliki tugas untuk menemukan mereka...",
                "created": "2011-02-08 08:33:33",
                "modified": "2014-01-28 14:41:05",
                "status": "publish",
                "type": "series",
                "cover_color": "#dddddd",
                "url": "http://api.ngomik.dev/v1/series/563",
                "permalink": "http://www.ngomik.com/comic/battleloid/563",
                "thumbnail": "http://www.ngomik.com/comic/thumb/id/563/width/200/height/300",
                "chapter_count": "2",
                "subscribed": 0,
                "author": {
                    "id": "1284",
                    "username": "sayakachan95",
                    "created": "2011-01-14 12:58:17",
                    "modified": "2012-09-26 02:49:24",
                    "last_activity": "2012-04-27 20:59:03",
                    "url": "http://api.ngomik.dev/v1/authors/1284",
                    "permalink": "http://www.ngomik.com/sayakachan95",
                    "avatar": "http://api.ngomik.dev/img/avatar/1284/100/100/1284.jpg",
                    "display_name": "Handayani F"
                }
            }
        ]
    }    
    
#### Detail
Mendapatkan informasi dari suatu series

##### url
v1/series/{id}

##### parameter
* **id**: ID series

##### contoh hasil
        
    {
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
        },
        "chapters": {
            // list of chapters
        }
    }