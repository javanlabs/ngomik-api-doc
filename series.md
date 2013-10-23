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
        "items":"[
            {\"id\":\"8171\",\"title\":\"komik baru\",\"description\":\"test\"},            
            {\"id\":\"8170\",\"title\":\"test\",\"description\":\"test\"}
        ]"
    }