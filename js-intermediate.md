<h1>JavaScript Intermediate</h1>

<h2>Object</h2>
<p>Object merupakan sebuah tipe data pada variable yang menyimpan properti dan fungsi</p>

```
let person = {}  //ini adalah object yang bernama person
```

<p> kita dapat menyimpan berbagai tipe data dalam object</p>

```
let person = {
  name: "Indah Storyna", //Properti daro object person
  age: 22,  //Properti daro object person
  address: Jereweh, Sumbawa Barat  //Properti daro object person
}

```

<hr>
<h2>.map()</h2>
<p>digunakan untuk melakukan perulangan sambil mengecek/melakukan operasi terhadap setiap elemen array, lalu memberikan nilai balik berupa array baru tanpa mengubah nilai pada array yang lama.</p>

<p>Callback function pada .map() memiliki 3 parameter dasar yang dapat digunakan sesuai kebutuhan:</p>

<li>value yaitu isi dari tiap elemen yang diproses.</li>
<li>index (optional) yaitu nomor index tiap elemen.</li>
<li>array (optional) yaitu array itu sendiri.</li>

<hr>

```
arr.map((value, index, array) => {
  // kode program
});
```

```
let input = [100, 50, 60, 10];

let output = input.map(item => {
  return item/10;
});

console.log(output);
// Output [10, 5, 6, 1]

console.log(input);
// Output [100, 50, 60, 10] --> Nilai array pertama tidak berubah
```

<h2>Rekursive</h2>

<p>Recursive adalah fungsi yang memanggil dirinya sendiri sampai kondisi tertentu.
</p>

```
function recursive(){
  if(condition) {
    //...
  }else {
    recursive();
  }
}
```

<p>Fungsi rekursif selalu memiliki kondisi yang menyatakan kapan fungsi tersebut berhenti.</p>

<p>Salah satu contohnya adalah mencari nilai pangkat</p>

```
function pow(x, n) {
  if (n == 1) {
    return x;
  }else{
    return x * pow(x,n-1);
  }
}
console.log(pow(2,3));
```
