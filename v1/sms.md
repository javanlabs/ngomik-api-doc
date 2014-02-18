### SMS

#### Generate Code (for authenticated user)
Meng-generate kode sms dan kode beli untuk keperluan pembelian via SMS.

##### url
v1/sms/generate_code (POST)

##### parameter
* **item_id**: ID item di ngomik.com

##### contoh hasil
     {
        "sms_code": "eiOn2SA",
        "purchase_code": "0VcIycY"
    }
    
#### Generate (for non authenticated user)
Meng-generate kode sms dan kode beli untuk keperluan pembelian via SMS.

##### url
v1/sms/generate (POST)

##### parameter
* **item_id**: ID komik di ngomik.com
* **item_title**: judul komik
* **item_price**: harga komik
* **param (array)**: tambahan informasi untuk keperluan logging

##### contoh hasil
    {"status":1,"sms_code":"ABCDEF","purchase_code":"GHIJKL"}