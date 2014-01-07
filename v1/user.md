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
    