### Author


#### Index
Mendapatkan list of author

##### url
v1/authors

##### parameter
* **order**: newest, oldest
* **limit**: berapa banyak item yang ingin diambil
* **page**: untuk menentukan mulai dari urutan keberapa item yang diambil

##### contoh hasil

    {
        "total": 53224,
        "per_page": 2,
        "current_page": 1,
        "last_page": 26612,
        "from": 1,
        "to": 2,
        "data": [
            {
                "id": "53338",
                "username": null,
                "created": "2014-01-07 08:50:49",
                "modified": "2014-01-07 08:50:49",
                "last_activity": null,
                "url": "http://localhost/ngomik-api/public/v1/authors/53338",
                "avatar": "http://www.ngomik.com/user/thumb/id/53338",
                "display_name": null
            },
            {
                "id": "53337",
                "username": null,
                "created": "2014-01-07 08:50:44",
                "modified": "2014-01-07 08:50:44",
                "last_activity": null,
                "url": "http://localhost/ngomik-api/public/v1/authors/53337",
                "avatar": "http://www.ngomik.com/user/thumb/id/53337",
                "display_name": null
            }
        ]
    }
    
#### Detail
Mendapatkan informasi dari author tertentu

##### url
v1/authors/{id}

##### parameter
* **id**: ID author

##### contoh hasil
        
    {
        "id": "53338",
        "username": null,
        "created": "2014-01-07 08:50:49",
        "modified": "2014-01-07 08:50:49",
        "last_activity": null,
        "url": "http://localhost/ngomik-api/public/v1/authors/53338",
        "avatar": "http://www.ngomik.com/user/thumb/id/53338",
        "display_name": null,
        "series": []
    }