# daniel.github.io

<html>
<meta charset='UTF-8'/><meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport'/><meta content='IE=edge' http-equiv='X-UA-Compatible'/>
<link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Quicksand&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script><link href="https://kado-untukmu.likeadream.repl.co/style.css" rel="stylesheet" type="text/css" /><script src="https://kado-untukmu.likeadream.repl.co/script.js"></script>
<head>
<!-- 
This code was made by Rayya R!
Blog: https://sinkronin.com
Instagram: @rayyarrr
TikTok: @rayyarr_
Telegram: @rayyarr
WhatsApp: 6282130626142
-->
</head>
<body>
<style>
body{background-image: url("https://i.postimg.cc/dtnfMN6c/IMG-20211103-181126-886.jpg");background-repeat: no-repeat;background-size: 105% 105%;animation:none;transition:all .3s ease;}
</style>
<div id='konten'><div class="foto"><div class="image">
<!-- Foto --><img id="ftKm" src="https://i.postimg.cc/0jyyvR8J/images.jpg" width="100px" height="100px" onClick="klikfoto();"/></div>
<span style="font-weight:700;font-size: 13px" id="sp1"><div id="lope" style="display:inline-block;align-items:center;justify-content:center;">&#9829;</div></span>
<div id="sp2" style="display:none;"><span style="font-weight:700;font-size: 13px" id="finish"></span></div>
</div>
<div id='scrollImage'>
  <p>Hai&nbsp;<b id="kamu"></b>&nbsp;manis ><</p>
  <p>Ciyeeeee</p>
  <p>yang hari ini ultah</p>
  <p>Panjang umur yaa</p>
  <p>Makin tua aja nih wkwk</p>
  <p>Candaa wlee<img style="margin-left:10px;" alt="Pentol" src="https://c.tenor.com/AlUwZp0ih_wAAAAi/pentol-quby.gif" height="70" /></p>
  <p>Oh iya</p>
  <p>Sehat selalu yaa</p>
  <p>Gak boleh males-malesan lagi</p>
  <p>Harus Makin rajin belajarnya</p>
  <p>Harus jadi yang lebih baik</p>
  <p><img style="margin-right:10px;" alt="Pentol" src="https://c.tenor.com/1Si3A6alsiEAAAAi/pentol-quby.gif" height="70" />
  Okeyy?</p>
  <p>Wish you all the best&nbsp;<span id="wrnRed">><</span></p>
  <p>Sekian &#10084;&#65039;</p>
  <p>Klik Foto di atas~<img style="margin-left:10px;" alt="Pentol" src="https://c.tenor.com/oQ_6wxtMrx0AAAAi/pentol-quby.gif" height="70" /></p>
</div></div>

<div id="contTom"><a class='button whatsapp' onClick='bukaWa();'><i class='icon whatsapp'></i>Kirim</a>
</div>

<script>  
var a=0,finish;
finish = "Selamat ulang tahun ya cantik❣️";

//Opsi WhatsApp
 function bukaWa(){window.location = "https://api.whatsapp.com/send?phone=&text=Hai, Aku " + "*" + nama + "*" + "%0A%0A" + "*" + nama + "*" + " udah bacain semuanya. Makasih yaaa" + " *" + author + "* " + "udah bikinin ini semua><" + "%0A%0A" + "*" + "Dikirim:" + "*" + "%20" + dateTime;} 
</script>
<script type="text/javascript">            
            var today = new Date();var date = today.getDate()+'/'+(today.getMonth()+1)+'/'+today.getFullYear()+'.';var dateTime = date;
            const swals = Swal.mixin({
                cancelButtonColor: '#909090',
                confirmButtonColor: '#00B487',
                allowOutsideClick: false,
            });
            async function mulai(){
                var { value: nama } = await swals.fire({
                    title: 'Nama kamu?',
                    input: 'text',
                    confirmButtonText: 'Lanjut',
                    showCancelButton: false,
                });                           
                if(nama){
                	window.nama = nama;
                    finish = finish + ", " + nama + "!";    
                    document.getElementById("kamu").innerHTML = "" + window.nama;                      
                	var { value: author } = await swals.fire({
                    title: nama + ' tau Aku siapa? Spill namanya dong!',
                    input: 'text',
                    confirmButtonText: 'Lanjut',
                    showCancelButton: false,
                    });                
                  if(author != nama){
                    document.getElementById("sp1").innerHTML = "Dari " + author + ", Untuk " + window.nama + "!";
                	window.author = author;                   
                    await swals.fire(`Sekarang lihat ini ya &#10084;&#65039;`);
                    setTimeout(showDiv, 100);                                    
               } else {
                    await swals.fire('Nama tidak boleh kosong/sama dengan nama kamu!');
                    mulai();
                }
                } else {
                    await swals.fire('Nama tidak boleh kosong, ya!');
                    mulai();
                }
            }
//funct Mulai
mulai()            
</script>
<script>
  function nonDiv() {document.getElementById('konten').style.opacity = "0";} function showDiv() {document.getElementById('konten').style.opacity = "1";document.getElementById('konten').style.top = "0";document.querySelector("body").style.animation = "anim 9s ease infinite";}
  function tombol() {document.getElementById('contTom').style.margin = "0";document.getElementById('contTom').style.opacity = "1";var e1 = document.getElementById('ftKm');e1.classList.add("degdeg");}  
  function klikfoto() {document.getElementById('sp1').style.display = "none";document.getElementById('sp2').style.display = "block";if(a<finish.length){document.getElementById("finish").innerHTML += finish.charAt(a);a++;setTimeout(klikfoto,100);} if(a==finish.length){setTimeout(tombol,500);}}
</script>
</body>
</html>
