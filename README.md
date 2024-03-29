# Pweb-Tugas2
Dibuat untuk memenuhi tugas matakuliah Praktikum Website 1

Mempelajari mengenai HTML, CSS, dan JavaScript
Untuk mengimplementasikan hal yang sudah dipelajari disini saya membuat list dengan html:
<h4>List Takjil:</h4>
            <ol>
                <li>
                    <ul>Makanan
                        <li>Risoles</li>
                        <li>Lapis Legit</li>
                        <li>Gorengan</li>
                        
                    </ul>
                </li>
                <li>Minuman
                    <ul>
                        <li>Es Teh</li>
                        <li>Es Buah</li>
                        <li>Es Kuwut</li>
                        
                    </ul>
                </li>
            </ol>
dengan code sebagai berikut yang mana h4 untuk membuat headings berukuran 4, ol untuk ordered list yang akan muncul angka, li untuk list, dan ul untuk unordered list

Lalu membuat tabel dari html dan didesain menggunakan css:
<style>
  #customers {
  font-family: Arial, Helvetica, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

#customers td, #customers th {
  border: 2px solid #75eb89;
  padding: 8px;
}

#customers tr:nth-child(even){background-color: #f2f2f2;}

#customers tr:hover {background-color: #ddd;}

#customers th {
  padding-top: 12px;
  padding-bottom: 12px;
  text-align: center;
  background-color: #04AA6D;
  color: white;
}
</style>
<h4>Tabel Mahasiswa 2</h4>
        <table id="customers"style="width:30%">
            <tr>
            <th colspan="2">Data Mahasiswa</th>
            </tr>
            <tr>
            <td>Alfreds Futterkiste</td>
            <td>Maria Anders</td>
            </tr>
            <tr>
            <td>Berglunds snabbköp</td>
            <td>Christina Berglund</td>
            </tr>
            <tr>
            <td>Berglunds snabbköp</td>
            <td rowspan="3"><img src="https://www.ferinahospital.com/wp-content/uploads/2018/06/gedung-ferina1.jpg" width="180px" height="150px"></td>
            </tr>
            <tr>
            <td>Berglunds snabbköp</td>
            </tr>
            <tr>
            <td>Berglunds snabbköp</td>
            </tr>
        </table>
Table dimulai dari membuka kurung table lalu diberi id customers dengan ukuran lebar 30%, adapun tr yaitu table row, th yaitu table header, dan td yaitu table data. karena menggunakan
id maka didalam style css memanggilnya menggunakan # didepan nama yang diberikan. Jika ingin menggabungkan beberapa coloum menggunakan colspan sebaliknya jika ingin menggabungkan row
menggunakan rowspan.

Lalu memanggil kata yang berada dalam tabel menggunakan JavaScript:
<h4>Table Mahasiswa 1</h4>
            <table style="width:30%">
        <tr>
            <th>Firstname</th>
            <th>NPM</th>
        </tr>
        <tr>
            <td id="a">Ferina</td>
            <td id="b">230302036</td>
        </tr>
        <tr>
            <td>Kate</td>
            <td>230102037</td>
        </tr>
        <tr>
            <td>Shela</td>
            <td>230303033</td>
        </tr>
        </table>

<br>
<script>
    let a = document.getElementById("a").innerHTML;
    let b = document.getElementById("b").innerHTML;
    let hasil = hitung (a,b);
    document.write("Nilai A adalah =" +a,"<br>");
    document.write("Nilai B adalah =" +b,"<br>");

    function hitung(a,b){
        return a*b;
    }
    
    function tampil(){
        alert("Hasil A+B=" + hasil)
    }
</script>
<button type="button" onclick="tampil()">Hitung</button>

Let a dan Let b digunakan untuk wadah menampung dari elemen id a dan elemen id b lalu let hasil yang akan dipanggil oleh function, document write digunakan untuk menuliskan nilai a itu
ada apa saja, button digunakan untuk mengklik lalu akan muncul alert yang digunakan untuk memunculkan hasilnya


  
