## Method Array Javascript

1. Method toString().
    metode mengembalikan string dengan semua nilai array, dipisahkan dengan koma

    Demo method array toString() javascript

    ```Javascript

    var array1 = [1, 2, 'halo', 'semua'];
    console.log(array1.toString());// expected output: "1,2,halo,semua"
    
    ```

2. Method join().
    membuat dan mengembalikan string baru dengan menggabungkan semua elemen dalam array (atau objek mirip array), dipisahkan dengan koma atau string pemisah yang ditentukan. Jika array hanya memiliki satu item, maka item itu akan dikembalikan tanpa menggunakan pemisah.
        
    Demo method array join() javascript

    ```Javascript
    
    var elements = ['Api', 'Air', 'Udara'];

    console.log(elements.join()); // expected output: "Api,Air,Udara"
    console.log(elements.join('')); // expected output: "ApiAirUdara"
    console.log(elements.join('-')); // expected output: "Api-Air-udara"
    
    ```
3. Method push().
    menambahkan satu atau lebih elemen ke akhir array dan mengembalikan panjang array yang baru.

    Demo method array push() Javascript

    ```Javascript

    var buah = ["Pisang", "Jeruk", "Apel", "Mangga"];
    fruits.push("Kiwi");
    console.log(fruits)

    ```
4. Method pop().
    metode menghapus elemen terakhir dari array dan mengembalikan elemen itu. Metode ini mengubah panjang array.

    Demo method array pop() Javascript

    ```Javascript

    var sayur = ['brokoli', 'kangkung', 'bayam', 'tomat'];
    console.log(sayur.pop()); // expected output: "tomat"
    console.log(sayur); // expected output: Array ["brokoli", "kangkung", "bayam"]

    ```

5. Method unshift().
    Metode unshift () menambahkan satu atau lebih elemen ke awal array dan mengembalikan panjang array yang baru.

    Demo method array unshift() Javascript

    ``` Javascript

        var array1 = [1, 2, 3];
        console.log(array1.unshift(4, 5)); // expected output: 5
        console.log(array1); // expected output: Array [4, 5, 1, 2, 3]
    
    ```
6. Method shift().
    menghapus elemen pertama dari array dan mengembalikan elemen yang dihapus. Metode ini mengubah panjang array.

    Demo method array shift() Javascript

    ``` Javascript

        var buah = ["Pisang", "Jeruk", "Apel", "Mangga"];
        buah.shift();
        console.log(buah) //  output ["Jeruk", "Apel", "Mangga"]
        console.log(buah.shift()) // output "Jeruk"

    ```

7. Method splice().
    mengubah konten array dengan menghapus atau mengganti elemen yang ada dan / atau menambahkan elemen baru

    Demo method array splice() Javascript

    ``` Javascript

        var fruits = ["Banana", "Orange", "Apple", "Mango"];
        fruits.splice(2, 0, "Lemon", "Kiwi");
        console.log(fruits) //output ["Banana", "Orange", "Lemon", "Kiwi", "Apple", "Mango"
    
    ```

8. Method concat().
    Metode ini berfungsi untuk menggabungkan 2 array menjadi 1 array.

    Demo method array concat() Javascript

    ``` Javascript

        var fruits = ['apel', 'banana', 'mango']
        var number = [1, 2, 3]

        var newArray = fruits.concat(number);
        console.log(newArray); // Output: ["apel", "banana", "mango", 1, 2, 3]
    
    ```
9. Method slice()
    mengembalikan elemen yang dipilih dalam array, sebagai objek array baru.
    
    Demo method array slice() Javascript

    ``` Javascript

        var animals = ['ant', 'bison', 'camel', 'duck', 'elephant'];
        console.log(animals.slice(2)); // expected output: Array ["camel", "duck", "elephant"]
        console.log(animals.slice(2, 4)); // expected output: Array ["camel", "duck"]
        console.log(animals.slice(1, 5)); // expected output: Array ["bison", "camel", "duck", "elephant"]

    ```
10. Method map()
    Metode ini berfungsi untuk membuat array baru sambil mengecek/melakukan operasi terhadap setiap elemen array.

    Demo method array map() Javascript

    ``` Javascript

    var angka = [1, 2, 3, 4, 5, 6, 7, 8, 9]; 
    // membuat array baru dari array angka untuk memeriksa apakah setiap elemennya bernilai habis dibagi 2 atau tidak
    var mapedArray = angka.map(item => item % 2 === 0);
    console.log(mapedArray); // output: [false, true, false, true, false, true, false, true, false]
    // membuat array baru dari array angka untuk melakukan operasi perkalian 2 pada setiap elemennya
    var multipleOfTwo = angka.map(e => e * 2);
    console.log(multipleOfTwo); // Output: [2, 4, 6, 8, 10, 12, 14, 16, 18]

    ```