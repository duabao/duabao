function initengahan(){
    kadoIn.style="display:none";ket.style="display:none";
    Content.style = "opacity:1;margin-top:0";
    bodyblur.style="opacity:.7";
    wallpaper.style="transform: scale(1.5);";
  }
  
  async function mulainama() {
    bodyblur.style="opacity:.7";
    wallpaper.style="transform: scale(1);";
    fotostiker.style="display:inline-flex;";setTimeout(ftmuncul,200);
    setTimeout(kethalo,500);
  }
  
  function ftmuncul(){if(ftganti==0){fotostiker.src = deffotostiker;} if(ftganti==1){fotostiker.src = fotostiker1.src;} if(ftganti==2){fotostiker.src = fotostiker2.src;} if(ftganti==3){fotostiker.src = fotostiker3.src;} if(ftganti==4){fotostiker.src = fotostiker4.src;} fotostiker.style="display:inline-flex;opacity:1;transform:scale(1)";}
  function fthilang(){fotostiker.style="display:inline-flex;opacity:1;transition:all .7s ease;transform:scale(.1)";}
  function jjfoto(){fotostiker.style.animation="rto .8s infinite alternate";}
  
  function bqmuncul(){bq.style = "position:relative;opacity:1;visibility:visible;transform: scale(1);margin-top:0";mulaiketik1();fungsi=1;}
  function bqhilang(){wallpaper.style="transform: scale(2);";bodyblur.style="opacity:.3";bq.style = "position:relative;transition:all .7s ease;";}
  function kethalo(){new TypeIt("#halo", {strings: ["" + vketikhalo], startDelay: 50, speed: 40, waitUntilVisible: true, afterComplete: function(){halo.innerHTML = vketikhalo;setTimeout(bqmuncul,200);},}).go();}
  function tombol(){wallpaper.style="transform: scale(1);";Tombol.style="opacity:1;transform: scale(1);";fungsi=1}
  document.getElementById("By").onclick = function() {if(fungsi==1){pertanyaan();} if(fungsi==2){menuju();}}
  async function menuju(){await swals.fire('Uci!', 'Nhớ liên hệ anhh nhaaa bấy biii , anhh có này tặng choo bbi nàa!', 'success');window.location = "https://cuongnobro.github.io/Baby/";}
  
  vketik1=kalimat.innerHTML;kalimat.innerHTML = "";
  function mulaiketik1(){
  new TypeIt("#kalimat", {
  strings: ["" + vketik1], startDelay: 400, speed: 20, cursor: false, deleteSpeed: 20, breakLines: false, waitUntilVisible: true, lifelike: true,
  afterComplete: function(){
    aktiopsL();
  },}).go();
  }
  
  opsLclick=0;opsLcheck=0;defopsL=opsL.innerHTML;
  document.getElementById("bq").onclick = function() {
    if(opsLclick==1){
      if(opsLcheck==1){setTimeout(aktipesan1,400);}
      if(opsLcheck==2){mulaiketik3();}
      if(opsLcheck==3){mulaiketik4();}
      if(opsLcheck==4){mulaiketik5();}
      if(opsLcheck==5){kethalo2();}
      otomatis();opsL.style.opacity="0";opsLclick=0;
    }
  }
  function aktiopsL(){opsL.innerHTML=defopsL;opsL.style.opacity=".8";opsLclick=1;opsLcheck+=1;}
  function gantiopsL(){opsL.innerHTML="[ Klik beberapa LOVE-nya ]";opsL.style.opacity=".8";}
  function otomatis(){kalimat.style="opacity:0";setTimeout(otolanj,400);}
  function otolanj(){kalimat.style="opacity:1";}
  function aktipesan1(){kalimat.innerHTML=pesan1.innerHTML;kolombaru.style="position:relative;opacity:1;transform:scale(1);";}
  vketik2=pesan2.innerHTML;vketik3=pesan3.innerHTML;
  function aktipesan2(){
  wallpaper.style="transform: scale(1.5);";
  kolombaru.style="";kalimat.innerHTML="";
  new TypeIt("#kalimat", {
  strings: ["" + vketik2, "" + vketik3], startDelay: 20, speed: 30, cursor: true, deleteSpeed: 30, breakLines: false, waitUntilVisible: true, lifelike: true,
  afterComplete: function(){
    kalimat.innerHTML=vketik3;setTimeout(aktipesan4,700);
  },}).go();
  }
  vketik4=pesan4.innerHTML;pesan4.innerHTML="";
  function aktipesan4(){
  wallpaper.style="transform: scale(1);";
  fthilang();ftganti=2;setTimeout(ftmuncul,300);
  new TypeIt("#pesan4", {
  strings: ["" + vketik4], startDelay: 1, speed: 52, cursor: true, waitUntilVisible: true, lifelike: true,
  afterComplete: function(){
    pesan4.innerHTML=vketik4;setTimeout(aktipesan5,700);
  },}).go();
  }
  vketik5=pesan5.innerHTML;pesan5.innerHTML="";
  function aktipesan5(){
  wallpaper.style="transform: scale(1.5);";
  fthilang();ftganti=3;setTimeout(ftmuncul,300);
  new TypeIt("#pesan5", {
  strings: ["" + vketik5], startDelay: 1, speed: 52, cursor: true, waitUntilVisible: true, lifelike: true,
  afterComplete: function(){
    pesan5.innerHTML=vketik5 + " ><";setTimeout(aktipesan6,700);
  },}).go();
  }
  vketik6=pesan6.innerHTML;pesan6.innerHTML="";
  function aktipesan6(){
  wallpaper.style="transform: scale(1);";
  fthilang();ftganti=4;setTimeout(ftmuncul,300);
  new TypeIt("#pesan6", {
  strings: ["" + vketik6], startDelay: 1, speed: 52, cursor: true, waitUntilVisible: true, lifelike: true,
  afterComplete: function(){
    pesan6.innerHTML=vketik6;setTimeout(tombol,400);
  },}).go();
  }
  var slov=0;
  document.getElementById("lv1").onclick = function() {lv1.style="opacity:0";slov+=1;this.onclick=null;checkslov();}
  document.getElementById("lv2").onclick = function() {lv2.style="opacity:0";slov+=1;this.onclick=null;checkslov();}
  document.getElementById("lv3").onclick = function() {lv3.style="opacity:0";slov+=1;this.onclick=null;checkslov();}
  document.getElementById("lv4").onclick = function() {lv4.style="opacity:0";slov+=1;this.onclick=null;checkslov();}
  function checkslov() {if(slov==4){kolombaru.style="position:relative;transform:scale(1)";fthilang();ftganti=1;setTimeout(ftmuncul,300);otomatis();setTimeout(aktipesan2,400);}}
  <!DOCTYPE html>
<html>
<meta charset='UTF-8'/><meta content='width=device-width, initial-scale=1, user-scalable=1, minimum-scale=1, maximum-scale=5' name='viewport'/><meta content='IE=edge' http-equiv='X-UA-Compatible'/>
  
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Shippori+Antique:wght@400;700&display=swap" rel="stylesheet">
  <link href="https://fonts.googleapis.com/css2?family=Dancing+Script&display=swap" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11.0.19/dist/sweetalert2.all.min.js"></script><link href="https://feeldreams.github.io/heibuka/style.css" rel="stylesheet" type="text/css" />
  <script src="https://unpkg.com/typeit@8.7.0/dist/index.umd.js"></script>
  
<head>
<title>Mylove</title>
<link rel="icon" type="image/x-icon" href="https://www.palingit.com/favicon.ico">
<meta name="description" content="HTML Replit Coding">
</head>
<body>
	
  
   <audio src="https://feeldreams.github.io/maimuna.mp3" id="linkmp3" class="sembunyi"></audio>
   
   <div id="bodyblur">
     <!-- Wallpaper --><img src="data:image/jpeg;base64,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" id="wallpaper"/><div id="beneranblur"></div>
   </div>
   
   <div id='Content'>
     <div id="kadoIn">
       <!-- Tombol Surat --><img src="https://feeldreams.github.io/kadoin.png"/>
     </div>
     <p id="ket">Mở quà đii bé iuu :3</p>
     <div class="kumpulanstiker">
         <!-- Stiker untuk Konten -->
         <img src="https://feeldreams.github.io/peach6.gif" id="fotostiker"/>
         <img src="https://feeldreams.github.io/bunga.gif" id="fotostiker1"/>
         <img src="https://feeldreams.github.io/pandacoklat.gif" id="fotostiker2"/>
         <img src="https://feeldreams.github.io/gumush.gif" id="fotostiker3"/>
         <img src="https://feeldreams.github.io/emawh.gif" id="fotostiker4"/>
         
         <img src="https://feeldreams.github.io/pandacoklat.gif" id="fotostiker5"/>
     </div>
     
     <p id="halo" class="halo"></p>
     
     <div><blockquote id='bq' data-text='💞'>
       <p id="kalimat">Hôm nay anh ở đây muốn nói với em một điều nhỏ nhoyy hoyy 👉👈</p>
       <!-- Pesan -->
       <p id="pesan1">Chạm đủ 4 love nhoo  ❤️</p>
       <div id="kolombaru">
         <li id="lv1"> ❤️</li>
         <li id="lv2"> ❤️</li>
         <li id="lv3"> ❤️</li>
         <li id="lv4"> ❤️</li>
       </div>
       <p id="pesan2">Tuỵt zờiiiii! 💘</p>
       <p id="pesan3">Anh muốn nóiii với em là là là.....</p>
       <p id="pesan4" class="sty2">Anh iuu emmm nhìu lắmmm lắm nhunnn</p>
       <p id="pesan5" class="sty2">hong biết aiii đó có nhớ anhhh khonnggg hàaaaa</p>
       <p id="pesan6" class="sty2">Còn anhh trong đầuuu bây giờ chỉ có hình póngg dáng em thoaii🤧</p>
       <!-- Tombol Lanjut -->
       <p id="opsL">Tiếp nàaaaa bbii</p>
     </blockquote></div>
     <!-- Tombol Kirim Pesan -->
     <div id="Tombol"><a id="By">&#128140; Click</a></div>
     
     <!-- Pesan Ditolak -->
     <div id="pesanditolak">
       <img id="stikerditolak" src="https://feeldreams.github.io/weee.gif"/>
       <p id="kataditolak">Bộ em thích từ chối lắm hả ? Nhưng mà em bị lừa rồiii cục cưng 😆</p>
     </div>
   </div>
<script>
  const body = document.querySelector("body");const swalst = Swal.mixin({timer: 2300, allowOutsideClick: false, showConfirmButton: false, timerProgressBar: true, imageHeight: 90,}); audio = new Audio('' + linkmp3.src); ftganti=0;fungsi=0;fungsiAwal=0;deffotostiker=fotostiker.src;Content.style = "opacity:1;margin-top:16vh"; const swals = Swal.mixin({allowOutsideClick: false, cancelButtonColor: '#FF0040', imageHeight: 80,}); 
  document.getElementById("kadoIn").onclick = function() {if(fungsiAwal==0){audio.play();fungsiAwal=1;kadoIn.style="transition:all .8s ease;transform:scale(10);opacity:0";wallpaper.style="transform: scale(1.5);";ket.style="display:none";setTimeout(initengahan,300);setTimeout(inipesan,500)}}
  
  async function inipesan(){
    var { value: nama } = await swals.fire({
           title: 'Tên của bé iuu là gì?', input: 'text',
       });
       if(nama && nama.length < 11){
         window.nama = nama;
         vketikhalo="Hai, " + nama + " 💑";
         mulainama();
         } else {
           await swals.fire('Bộ em hong có tên hả!', 'Tên của người đẹp chỉ chứa 10 ký tự hoii nhaaa, ya!');inipesan();
    }
  }
  
  var tanya = 'có rảnh hongg nói chuyện với anh chút nhéee 😳';
  var opstanya = 'Lựa chọn của em là......';
  var tompositif = 'Em đồng ý';
  var tomnegatif = 'Em hong chịu';
  
  async function pertanyaan(){var { isConfirmed: prtanya } = await swals.fire({title: nama + ' ' + tanya, text: '' + opstanya, imageUrl: '' + fotostiker5.src, showCancelButton: true, confirmButtonText: '' + tompositif, cancelButtonText: '' + tomnegatif,});
    if(prtanya){
	pesanwhatsapp = "Iyaa " + nama + " kangen kamu juga kok! ><";
	menuju();
    } else {
	pesanwhatsapp = nama + " engga kangen kamu wleee! :p";
	await swalst.fire({title: '' + kataditolak.innerHTML, timer: 2000, imageUrl: '' + stikerditolak.src,});
	menuju();
    }
    }
</script>
<script src="a.js"></script>
</body>
</html>
:root {
    --tombol-bg: rgba(0, 0, 0, .3); 
    --tombol-teks: #fff;
    --tombol-bingkai: #fff;
    --bingkai: 8px;
    --bingkai-kiri: 1.3px solid var(--tombol-bingkai);
    --bingkai-kanan: 1.3px solid var(--tombol-bingkai);
    --gaya-font: 'Shippori Antique', sans-serif;
    --gaya-font2: 'Dancing Script', sans-serif;
    }
    @keyframes fanim {0% {background-position: 0% 0%;}25% {background-position: 100% 100%;} 50% {background-position: 0% 100%;} 75% {background-position: 50% 50%;} 100% {background-position: 0% 0%;}}
    body{background-color:#000;font-family:var(--gaya-font);padding: 20px 25px;-webkit-user-select: none; -ms-user-select: none; user-select: none;} a{text-decoration:none;}
    body::before{content:"\00A9  Rayys | PalingIT";color:white;opacity:.05;font-size:10px;position:fixed;bottom:25px;right:25px;z-index:2}
    #bodyblur{opacity:0;position:fixed;top:0;left:0;right:0;bottom:0;background:rgba(0,0,0,.3);transition:all 1s ease;} 
    #wallpaper{width:100%;height:100%;transform: scale(2);transition:all 1.3s ease;}
    #beneranblur{position:fixed;top:0;left:0;right:0;bottom:0;background:rgba(0,0,0,.3);-webkit-backdrop-filter:blur(0px); backdrop-filter:blur(0px);transition:all 3s ease;}
    
    @keyframes jj{0%  {transform: scale(1.1);} 50% {transform: scale(1.2);} 100% {transform: scale(1.1);}}
    @keyframes rts{from {transform:scale(.1);} to {transform:scale(1);}}
    @keyframes rto{from {transform:scale(1);} to {transform:scale(1.1);}}
    @keyframes aniopa{0% {transform: scale(1);} 50% {transform: scale(.75);} 100% {transform: scale(1);}}
    @keyframes rtf{from {transform: rotate(0deg);} to {transform: rotate(360deg);}} @keyframes rt{from {transform: scale(.9);/* transform: rotate(-5deg); */} to {transform: scale(1);/* transform: rotate(5deg); */}}
    @keyframes kont{0%  {left:-1px; top:-3px;} 50% {left:1px; top:3px;} 100% {left:-1px; top:-3px;}}
    
    blockquote{position:absolute;opacity:0;visibility:hidden;margin-top:100px;background:var(--tombol-bg);border-radius:18px 0 18px 0;box-shadow: rgba(255,255,255, 0.3) 0px 7px 29px 0px;transform: scale(.1);transition:all 1s ease;margin-top:120px;margin-left:0;margin-right:0;color:var(--tombol-teks);text-shadow: 0px 2px 2px rgba(0, 0, 0, .8);}
    blockquote{width:400px;text-align:center;line-height:1.3em;padding:20px 25px 20px 25px;}
    blockquote::before{content:attr(data-text);opacity:.7;font-family: sans-serif;position:absolute;left:8px;top:8px;min-width:15px;font-size:16px;text-align:center}
    blockquote::after{content: "";position: absolute;border: 1px solid #fff;border-radius:18px 0 18px 0;top: -8px;bottom: -8px;left: -8px;right: -8px;}
    blockquote p{font-size:16px;font-weight:700;line-height:1.4em;transition:all .5s ease;}
    blockquote > #kalimatb, blockquote > .sty2{font-size:15px;font-weight:400}
    blockquote > #pesan4{margin-top:25px} blockquote > .sty2{line-height:1em;}
    blockquote p:not(#opsL, #kalimat, #kalimatb, .sty2){display:none;}
    blockquote > #opsL{text-align:right;font-size:11px;font-weight:400;line-height:0;margin-top:24px;color:white;opacity:0;transition:all .2s ease;}
    
    #waktu{display:none}
    #kado1, #kado2, #kado3{font-size:16px;font-weight:400;}
    #kalimatAkhir{transform:scale(.1);}
    #kado1{position:absolute;opacity:0}
    #kalove{font-size:25px;line-height:0;}
    .kolombar .inibar{position:absolute;opacity:0;visibility:hidden;background-color:#fff;height:5px;width:100%}
    
    #Tombol{position:relative;opacity:0;margin:0;display:flex;align-items:left;list-style:none;transform: scale(.1);transition:all 1s ease;}
    #Tombol a{cursor:pointer;display:inline-flex;align-items:center; margin:0;margin:12px 0 12px 0;transition:all .2s ease;padding:10px;outline:0;border: 1px solid #fff;border-radius:18px;line-height:15px;background:rgba(0,0,0,.5);color:var(--tombol-teks);font-size:12px;font-weight:700;white-space:nowrap;overflow:hidden;box-shadow: rgba(255,255,255, 0.3) 0px 7px 29px 0px;z-index:1} 
    #Bn{margin:12px 0 12px 12px !important;}
    #Bn2{position:absolute;opacity:0;width:0}
    
    #Content{animation-name:none;animation-duration: 3s;animation-iteration-count: infinite;position:relative;opacity:0;margin-top:50px;width:100%;height:180px;transition:all .7s ease;}
    #Content > *{display:flex;align-items:center;text-align:center;justify-content:center;margin-top:1px;}
    .kumpulanstiker > img{display:none;background: rgba(255, 255, 255, 0.2);box-shadow: 0 4px 30px rgba(255,255,255, 0.3);backdrop-filter: blur(5px);-webkit-backdrop-filter: blur(5px);border: 1px solid rgba(255, 255, 255, 0.3);border-radius: 50%;padding:10px;width:100px;height:100px;margin:20px 0;}
    #fotostiker{opacity:.1;transition:all 1.2s ease;transform: scale(.1);}
    .halo{font-size:18px !important;position:relative;margin:15px 0 20px 0} 
    .halo.sty2{font-family:var(--gaya-font2);font-size:24px !important;margin-top:20px !important;}
    .halo.sty3{position:absolute !important;font-size:14px !important;font-weight:400 !important;margin:30px 20px !important;}
    #kalimatbawah{position: absolute;opacity:0;transform: scale(.3);margin:50px 0;font-family:var(--gaya-font2);font-size:20px;font-weight:700;color:white;text-shadow: 0px 2px 2px rgba(0, 0, 0, .8);transition:all .5s ease;}
    #tanggal{position: absolute;opacity:0;transform: scale(.3);transition:all .5s ease;}
    
    #fotolove img{transition:all .5s ease;width:75px;height:75px;padding:0;background:none}
    #kadoIn img{display:inline-flex;background:none;width:130px;height:130px;transition:all .3s ease;} 
    #ket, .halo{text-shadow: 0px 2px 2px rgba(0, 0, 0, .8);font-size:17px;font-weight:700;color:white}
    #ket{margin-top:25px !important;font-weight:400;}
    #kadoIn img:hover{transform:scale(.9);}
    
    #kolombaru{position:absolute;opacity:0;display:flex;transform:scale(.1);transition:all 1s ease;align-items:center;text-align:center;justify-content:center;z-index:1;}
    #kolombaru > li{margin:8px;padding:0;list-style-type: none;}
    #kolombaru li{opacity:.8;display:flex;font-size:30px}
    #kolombaru li:hover{opacity:.5;transform: scale(1.15);transition:all .3s ease;}
    
    .kolomrange{padding:0;background:none;position:relative;z-index:1;display:none;transition:all 1s ease;align-items:center;}
    .kolomrange .inirange{width:100%;height:40px;margin-right:15px;display:flex;align-items:center;text-align:center;justify-content:center;}
    .kolomrange .inirange input{height:10px;width:100%;-webkit-appearance:none;outline:none;background:#f2f2f2;border-radius:25px;box-shadow:inset 0px 0px 4px rgba(0,0,0,0.2);}
    .kolomrange .inirange input::-webkit-slider-thumb{-webkit-appearance:none;appearance:none;width:20px;height:20px;border-radius:50%;border:3px solid #006FFF;background:white;transition:all .2s ease;}
    .kolomrange .inirange input::-webkit-slider-thumb:hover{border:5px solid #006FFF;}
    .kolomrange .inivalue{color:white;font-size:20px}
    
    .swal2-modal > *{font-size:16px;}
    .swal2-title{line-height:1.3em;font-size:17px;text-align:center;padding:15px 30px 0 30px;}
    .swal2-timer-progress-bar-container > *{opacity:.7;background:#00B6FF;margin:0 2px}
    .swal2-modal{background:#EAEAEA;box-shadow: 0 4px 30px rgba(255,255,255, 0.3);backdrop-filter: blur(2px);-webkit-backdrop-filter: blur(2px);border: 1px solid rgba(255, 255, 255, 0.3);border-radius: 8px;max-width:330px;top:-60px;}
    .swal2-styled.swal2-confirm, .swal2-styled.swal2-cancel{position: relative;background-color: #4839eb;color: #fff;border-radius:18px;z-index: 1;transition: all 0.2s;}
    
    .fa-snowflake {opacity:.3;color:white;font-size: 20px;position: absolute;animation:  heartMove linear 1;top: -10vh;z-index: 0;}
    @keyframes heartMove {0%{transform: translateY(-10vh) ;} 100%{transform: translateY(100vh) ;}}
    .sembunyi, #pesanditolak > *, #kado2, #kado3{display:none !important}
