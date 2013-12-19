### Series

#### tipe
public

#### deskripsi
Mendapatkan list of series (series adalah kumpulan chapter).

#### url
series

#### parameter
* **order**: newest, oldest
* **take**: berapa banyak item yang ingin diambil
* **skip**: untuk menentukan mulai dari urutan keberapa item yang diambil

#### contoh pemanggilan
`series?order=newest&take=5&skip=5`

API di atas akan mengembalikan list of series **terbaru** sebanyak **5 item** dimulai dari **record ke 6** (karena 5 record pertama di-skip).

#### contoh hasil
    {
       "status":1,
       "count":2,
       "items":[
          {
             "id":11884,
             "title":"Urmarind Lumina ~mengejar cahaya~",
             "description":"komik curhat ane, setelah masuk kuliah ane mendapatkan pacar ane direbut org, dan sakit hati yang sangat mendalam mendorong saya untuk membuat komik ini demi merebut nya kembali!"
          },
          {
             "id":11883,
             "title":"eru ",
             "description":"kisah seorang pemuda yang melakukan travel time demi mencari benda pusaka desa yang hilang"
          }
       ]
    }