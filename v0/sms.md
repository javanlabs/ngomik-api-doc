### Request

#### tipe
private

#### desripsi
Meng-generate kode sms dan kode beli untuk keperluan pembelian via SMS.

#### url
sms/request

#### parameter
* **item_id**: ID komik di ngomik.com
* **item_title**: judul komik
* **item_price**: harga komik
* **param (array)**: tambahan informasi untuk keperluan logging

#### contoh pemanggilan
`sms/request?item_id=1&item_price=2000&item_title=title&app_id=123&app_secret=abc&param[email]=uyab@me.com&param[device]=samsung`

#### contoh hasil
    {"status":1,"sms_code":"ABCDEF","purchase_code":"GHIJKL"}