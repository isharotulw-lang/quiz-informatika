<!doctype html>
<html lang="id">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Quiz Informatika — Online</title>
<style>
  body { font-family: Arial, sans-serif; background:#f5f7fa; margin:0; padding:20px; }
  .container { max-width:900px; margin:auto; background:#fff; padding:20px; border-radius:10px; box-shadow:0 4px 10px rgba(0,0,0,0.1); }
  h1 { text-align:center; }
  .question-box { margin-bottom:20px; padding:15px; border:1px solid #ddd; border-radius:8px; }
  .question { font-weight:bold; margin-bottom:10px; }
  .result { margin-top:20px; padding:15px; background:#e3f7df; border-left:6px solid #3cb043; border-radius:6px; display:none; }
  button { padding:10px 20px; border:none; background:#3cb043; color:white; font-size:16px; border-radius:6px; cursor:pointer; }
  button:hover { background:#2e8b35; }
</style>
</head>

<body>
<div class="container">
<h1>Quiz Informatika</h1>
<p>Jawab semua soal kemudian klik tombol **Lihat Nilai**.</p>

<form id="quizForm"></form>

<button onclick="calculateScore()">Lihat Nilai</button>

<div class="result" id="resultBox"></div>

</div>

<script>
// =============== DATA SOAL ===============
const questions = [
  {type:"mcq", q:"Simbol flowchart untuk Start/End adalah...", choices:["Parallelogram","Diamond","Oval","Persegi panjang"], answer:2},
  {type:"mcq", q:"Simbol flowchart untuk proses adalah...", choices:["Persegi panjang","Oval","Parallelogram","Diamond"], answer:0},
  {type:"mcq", q:"Search engine berikut adalah...", choices:["Google","Microsoft Word","VLC","Photoshop"], answer:0},
  {type:"short", q:"Apa fungsi tombol Refresh di browser?", answer:["memuat ulang halaman","muat ulang","reload"]},
  {type:"short", q:"Apa itu file? Jawab singkat.", answer:["unit penyimpanan data","berkas"]},
  {type:"mcq", q:"Tombol keyboard untuk menyalin file adalah...", choices:["Ctrl+C","Ctrl+V","Ctrl+X","Ctrl+P"], answer:0},
  {type:"mcq", q:"Kotak Compose pada email digunakan untuk...", choices:["Menulis pesan baru","Membaca pesan","Menghapus pesan","Spam"], answer:0},
  {type:"mcq", q:"Format email yang benar adalah...", choices:["username@domain","domain@username","username#domain","username.domain"], answer:0},
  {type:"short", q:"KKM 75. Nilai 80 dinyatakan...?", answer:["lulus"]},
  {type:"mcq", q:"Aplikasi untuk membuka HTML adalah...", choices:["Browser","Antivirus","Photoshop","Excel"], answer:0},

  // ------- Tambahan (hingga 40 soal) --------
  {type:"short", q:"Sebutkan 4 pilar computational thinking.", answer:["dekomposisi, pola, abstraksi, algoritma","dekomposisi,pola,abstraksi,algoritma"]},
  {type:"mcq", q:"Komponen utama AAS adalah...", choices:["Sumber radiasi & atomizer","Sensor panas","Motor listrik","Baterai"], answer:0},
  {type:"mcq", q:"Flowchart adalah representasi...", choices:["visual dari algoritma","kode program","hardware","database"], answer:0},
  {type:"short", q:"Fungsi bookmark di browser?", answer:["menandai halaman","menyimpan alamat"]},
  {type:"mcq", q:"Graphite Furnace AAS digunakan untuk...", choices:["Jejak logam","Gambar","Teks","Video"], answer:0},
  {type:"short", q:"Sebutkan dua aplikasi AAS.", answer:["analisis logam berat, analisis pangan","analisis logam berat"]},
  {type:"mcq", q:"Simbol flowchart keputusan adalah...", choices:["Diamond","Oval","Parallelogram","Persegi"], answer:0},
  {type:"mcq", q:"Browser yang benar adalah...", choices:["Chrome","Word","Excel","Canva"], answer:0},
  {type:"short", q:"Apa itu ekstensi file?", answer:["penanda tipe file","format file"]},
  {type:"mcq", q:"Kelemahan AAS adalah...", choices:["Satu unsur per analisis","Banyak unsur sekaligus","Tidak selektif","Tidak sensitif"], answer:0},

  // 20 more (biar jadi 40)
  {type:"short", q:"Sebutkan 2 contoh sistem operasi.", answer:["windows, linux","android, windows"]},
  {type:"mcq", q:"RAM berfungsi untuk...", choices:["Menyimpan data sementara","Mencetak","Memutar video","Menyalin file"], answer:0},
  {type:"mcq", q:"CPU adalah...", choices:["Otak komputer","Layar","Speaker","Mouse"], answer:0},
  {type:"short", q:"Apa fungsi tombol Back?", answer:["kembali ke halaman sebelumnya","back"]},
  {type:"mcq", q:"Folder digunakan untuk...", choices:["Mengelompokkan file","Menjalankan internet","Menghapus virus","Merekam suara"], answer:0},
  {type:"short", q:"Apa kepanjangan WWW?", answer:["world wide web"]},
  {type:"mcq", q:"Jenis file gambar adalah...", choices:["PNG","DOCX","XLSX","PPTX"], answer:0},
  {type:"short", q:"Apa itu hardware?", answer:["perangkat keras"]},
  {type:"mcq", q:"Software untuk mengetik adalah...", choices:["Word","Chrome","Paint","Zoom"], answer:0},
  {type:"short", q:"Fungsi Save As?", answer:["menyimpan dengan nama baru","save as"]},

  // Final 10
  {type:"mcq", q:"Shortcut paste adalah...", choices:["Ctrl+V","Ctrl+C","Ctrl+S","Ctrl+A"], answer:0},
  {type:"mcq", q:"Shortcut seleksi semua adalah...", choices:["Ctrl+A","Ctrl+P","Ctrl+X","Ctrl+D"], answer:0},
  {type:"mcq", q:"Yang termasuk output device adalah...", choices:["Printer","Keyboard","Mouse","Scanner"], answer:0},
  {type:"short", q:"Browser apa yang dibuat Mozilla?", answer:["firefox"]},
  {type:"short", q:"Sebutkan 1 jenis memori komputer.", answer:["ram","rom"]},
  {type:"short", q:"Apa fungsi Address Bar?", answer:["mengetik alamat situs","alamat situs"]},
  {type:"mcq", q:"Perangkat untuk input adalah...", choices:["Keyboard","Monitor","Speaker","Proyektor"], answer:0},
  {type:"mcq", q:"File .mp3 adalah file...", choices:["Audio","Gambar","Dokumen","Spreadsheet"], answer:0},
  {type:"short", q:"Apa itu algoritma?", answer:["langkah-langkah penyelesaian masalah"]},
  {type:"mcq", q:"Program untuk browsing adalah...", choices:["Edge","Excel","Word","Notepad"], answer:0}
];

// ============================================
window.onload = function(){
  const quizForm = document.getElementById("quizForm");
  questions.forEach((q,i)=>{
    let box = `<div class="question-box">
      <div class="question">${i+1}. ${q.q}</div>
    `;
    if(q.type==="mcq"){
      q.choices.forEach((c,j)=>{
        box += `<label><input type="radio" name="q${i}" value="${j}"> ${c}</label><br>`;
      });
    } else {
      box += `<input type="text" name="q${i}" style="width:100%; padding:8px;">`;
    }
    box += `</div>`;
    quizForm.innerHTML += box;
  });
};

function calculateScore(){
  let score = 0;
  let total = questions.length;

  questions.forEach((q,i)=>{
    let val = document.querySelector(`[name="q${i}"]${q.type==="mcq" ? ":checked" : ""}`);
    if(!val) return;

    let ans = val.value.toString().toLowerCase().trim();

    if(q.type==="mcq"){
      if(Number(ans) === q.answer) score++;
    } else {
      let correct = false;
      q.answer.forEach(a=>{
        if(ans === a.toLowerCase()) correct = true;
      });
      if(correct) score++;
    }
  });

  let percent = Math.round((score/total)*100);
  document.getElementById("resultBox").style.display="block";
  document.getElementById("resultBox").innerHTML = `
    <h3>Hasil Anda:</h3>
    <strong>${score} / ${total}</strong> benar (${percent}%)
  `;
}
</script>

</body>
</html>
# quiz-informatika
