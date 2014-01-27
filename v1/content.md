### Content


#### Index
Mendapatkan list of contents

##### url
v1/contents

##### parameter
* **order**: newest, oldest
* **limit**: berapa banyak item yang ingin diambil
* **page**: untuk menentukan mulai dari urutan keberapa item yang diambil

##### contoh hasil
    {
        "status": 1,
        "chapters": {
            "total": 12632,
            "per_page": 2,
            "current_page": 1,
            "last_page": 6316,
            "from": 1,
            "to": 2,
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
                },
                {
                    "id": "2",
                    "title": "Speedy oh Speedy",
                    "slug": "speedy-oh-speedy",
                    "created": "2010-09-02 09:52:48",
                    "modified": "2012-09-11 09:19:15",
                    "published": "2010-09-02 02:52:48",
                    "url": "http://localhost/ngomik-api/public/v1/chapters/2",
                    "thumbnail": "http://www.ngomik.com/comicPage/thumb/comic_id/2/page_number/1",
                    "page_count": "1",
                    "synopsis": "",
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
        },
        "series": {
            "total": 8121,
            "per_page": 2,
            "current_page": 1,
            "last_page": 4061,
            "from": 1,
            "to": 2,
            "data": [
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
                    }
                },
                {
                    "id": "3",
                    "slug": "friends",
                    "title": "Friends",
                    "description": "disaat kita bersama~ diwaktu kita tertawa, menangis, merenung, oleh cinta~ jreng jreng jreng jreeng~ jreng jreng!!",
                    "created": "2010-09-02 09:50:26",
                    "modified": "2010-10-21 10:19:29",
                    "url": "http://localhost/ngomik-api/public/v1/series/3",
                    "thumbnail": "http://www.ngomik.com/comic/thumb/id/3/width/200/height/300",
                    "chapter_count": "2",
                    "author": {
                        "id": "5",
                        "username": "ardhan",
                        "created": "2010-08-24 16:09:37",
                        "modified": "2013-11-09 17:09:22",
                        "last_activity": "2012-09-27 07:35:20",
                        "url": "http://localhost/ngomik-api/public/v1/authors/5",
                        "avatar": "http://www.ngomik.com/user/thumb/id/5",
                        "display_name": "ardhan"
                    }
                }
            ]
        }
    }
    
#### Showcase
Mendapatkan konten pilihan untuk ditampilkan di halaman depan

##### url
v1/contents/showcase

##### parameter
* **limit**: berapa banyak item yang ingin diambil
* **page**: untuk menentukan mulai dari urutan keberapa item yang diambil

##### contoh hasil
    {
        "status": 1,
        "subscription_update": [//list of chapter object],
        "all_update": [//list of chapter object],        
        "top_series": [//list of series object],        
        "recommendation": [//list of series object],                
        "chapters": {
            "total": 12632,
            "per_page": 2,
            "current_page": 1,
            "last_page": 6316,
            "from": 1,
            "to": 2,
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
                },
                {
                    "id": "2",
                    "title": "Speedy oh Speedy",
                    "slug": "speedy-oh-speedy",
                    "created": "2010-09-02 09:52:48",
                    "modified": "2012-09-11 09:19:15",
                    "published": "2010-09-02 02:52:48",
                    "url": "http://localhost/ngomik-api/public/v1/chapters/2",
                    "thumbnail": "http://www.ngomik.com/comicPage/thumb/comic_id/2/page_number/1",
                    "page_count": "1",
                    "synopsis": "",
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
        },
        "series": {
            "total": 8121,
            "per_page": 2,
            "current_page": 1,
            "last_page": 4061,
            "from": 1,
            "to": 2,
            "data": [
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
                    }
                },
                {
                    "id": "3",
                    "slug": "friends",
                    "title": "Friends",
                    "description": "disaat kita bersama~ diwaktu kita tertawa, menangis, merenung, oleh cinta~ jreng jreng jreng jreeng~ jreng jreng!!",
                    "created": "2010-09-02 09:50:26",
                    "modified": "2010-10-21 10:19:29",
                    "url": "http://localhost/ngomik-api/public/v1/series/3",
                    "thumbnail": "http://www.ngomik.com/comic/thumb/id/3/width/200/height/300",
                    "chapter_count": "2",
                    "author": {
                        "id": "5",
                        "username": "ardhan",
                        "created": "2010-08-24 16:09:37",
                        "modified": "2013-11-09 17:09:22",
                        "last_activity": "2012-09-27 07:35:20",
                        "url": "http://localhost/ngomik-api/public/v1/authors/5",
                        "avatar": "http://www.ngomik.com/user/thumb/id/5",
                        "display_name": "ardhan"
                    }
                }
            ]
        }
    }