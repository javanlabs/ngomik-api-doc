### Subscription


#### List
Mendapatkan kode berlangganan user dan daftar berlangganan yang tersedia

##### url
v1/subscription/list (GET)

##### contoh hasil

    {
        "subscription_code":"55DM",
        "list":[
            {
                "operator":"Indosat",
                "shortcode":"99800",
                "data":[
                    {
                        "keyword":"REG NGOMIK",
                        "name":"7 Hari",
                        "duration":"1 week",
                        "price":2000,
                        "currency":"IDR"
                    }
                ]
            },
            {
                "operator":"Telkomsel",
                "shortcode":"92969",
                "data":[
                    {
                        "keyword":"REG NGOMIK",
                        "name":"7 Hari",
                        "duration":"1 week",
                        "price":2000,
                        "currency":"IDR"
                    }
                ]
            }
            ,
            {
                "operator":"XL\/AXIS",
                "shortcode":"92969",
                "data":[
                    {
                        "keyword":"REG NGOMIK",
                        "name":"7 Hari",
                        "duration":"1 week",
                        "price":2000,
                        "currency":"IDR"
                    }
                ]
            },
            {
                "operator":"3",
                "shortcode":"9296",
                "data":[
                    {
                        "keyword":"REG NGOMIK",
                        "name":"7 Hari",
                        "duration":"1 week",
                        "price":2000,
                        "currency":"IDR"
                    }
                ]
            }
        ]
    }