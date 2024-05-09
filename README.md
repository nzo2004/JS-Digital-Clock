Bu uygulama, Javascript kullanılarak oluşturulmuş basit bir saattir. Her saniye güncellenerek, size güncel saati gösterir.

var now = new Date(); = Anlık genel zaman bilgisini çekmek için kullanılır
var hour= now.getHours(); = Anlık saati alıyoruz.
var minute=now.getMinutes(); = Anlık dakika alıyoruz.
var second= now.getSeconds(); = Anlık saniye alıyoruz.

var day=now.getDate(); = Anlık gün bilgisi alınır
var month=now.getMonth()+1; = Anlık ay bilgisi ama array 0 dan başladığı için +1 ekleriz
var year= now.getFullYear(); = Anlık yıl bilgisi alınır

//1 saniyede 1 fonksiyonu tekrarlamak için kullanılır
//1000 = 1 saniyedir
//setInterval = kendini belirli zaman ile tekrarlayan fonksiyondur
setInterval(function(){GetTime();},1000);
