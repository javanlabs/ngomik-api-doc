### Categories


#### Index
Mendapatkan list of categories

##### url
v1/categories

##### parameter
* **type**: 'all', 'comic', 'artwork', 'story' (default 'all')

##### contoh hasil

    {
        "total": 11,
        "per_page": 100,
        "current_page": 1,
        "last_page": 1,
        "from": 1,
        "to": 11,
        "data": [
            {
                "id": "1",
                "slug": "action",
                "name": "Action",
                "type": "comic",
                "position": "1"
            },
            {
                "id": "2",
                "slug": "comedy",
                "name": "Comedy",
                "type": "comic",
                "position": "2"
            },
            {
                "id": "3",
                "slug": "fantasy",
                "name": "Fantasy",
                "type": "comic",
                "position": "3"
            },
            {
                "id": "4",
                "slug": "horror",
                "name": "Horror/Mystery",
                "type": "comic",
                "position": "4"
            }
        ]
    }