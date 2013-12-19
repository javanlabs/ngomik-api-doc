### Statistic


#### Summary
Mendapatkan ringkasan informasi jumlah konten yang tersedia.

##### url
v1/statistic/summary

##### parameter
none

##### contoh hasil
    {
        "status": 1,
        "total_user": "53212",
        "total_chapter": "8013",
        "total_artwork": "30673",
        "total_story": "2856"
    }
    
    
#### Daily Registration
Mendapatkan statistik jumlah registrasi user baru setiap hari dalam periode tertentu.

##### url
v1/statistic/registration

##### parameter
* **from**: tanggal awal (yyyy-mm-dd)
* **to**: tanggal akhir (yyyy-mm-dd)

##### contoh hasil

    {
        "status": 1,
        "from": "2012-07-01",
        "to": "2012-07-02",
        "day_count": "2",
        "daily_registration": {
            "2012-07-01": {
                "total": "155",
                "active": "106",
                "not_active": "49",
                "already_login": "87",
                "facebook": "53",
                "referral": "3"
            },
            "2012-07-02": {
                "total": "164",
                "active": "118",
                "not_active": "46",
                "already_login": "103",
                "facebook": "68",
                "referral": "6"
            }
        }
    }
    
#### Daily Publication
Mendapatkan statistik jumlah publikasi konten baru setiap hari dalam periode tertentu.

##### url
v1/statistic/publication

##### parameter
* **from**: tanggal awal (yyyy-mm-dd)
* **to**: tanggal akhir (yyyy-mm-dd)

##### contoh hasil

    {
        "status": 1,
        "from": "2012-07-01",
        "to": "2012-07-02",
        "day_count": "2",
        "daily_publication": {
            "2012-07-01": {
                "comic": "16",
                "artwork": "87",
                "story": "8"
            },
            "2012-07-02": {
                "comic": "15",
                "artwork": "113",
                "story": "4"
            }
        }
    }
    
#### Daily Reader
Mendapatkan statistik jumlah pembaca konten setiap hari dalam periode tertentu.

##### url
v1/statistic/reader

##### parameter
* **from**: tanggal awal (yyyy-mm-dd)
* **to**: tanggal akhir (yyyy-mm-dd)

##### contoh hasil

    {
        "status": 1,
        "from": "2012-07-01",
        "to": "2012-07-02",
        "day_count": "2",
        "daily_reader": {
            "2012-07-01": {
                "comic": "6229",
                "story": "902",
                "artwork": 0
            },
            "2012-07-02": {
                "comic": "10148",
                "story": "1180",
                "artwork": 0
            }
        }
    }