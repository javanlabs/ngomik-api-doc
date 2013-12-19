### List

#### tipe
public

#### deskripsi
Mendapatkan list of aplikasi mobile apps yang disediakan ngomik.com.

#### url
app/list

#### parameter
* **exclude**: ID atau list of ID app yang tidak ingin ditampilkan.

#### contoh pemanggilan
`app/list?exclude=1,2`

#### contoh hasil
    {
       "status":1,
       "apps":[
          {
             "id":"1",
             "title":"Kimong Legend #1",
             "description":"Desa Himong yang terkenal.",
             "author":"hadiruto",
             "app_url":"https:\/\/play.google.com\/store\/apps\/details?id=com.ngomik.kimonglegend.chapter1",
             "cover_url":"https:\/\/dl.dropboxusercontent.com\/u\/21271348\/ngomik\/cover%20apps\/kimong-chap1.png",
             "royalti_share":"0",
             "created":"2013-10-21 10:48:13",
             "modified":"2013-10-21 10:48:13"
          }
       ]
    }