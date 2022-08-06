<div align = "center">
  <h1> Deret Fibonacci Java </h1>
</div>

Deret angka sederhana yang penjumlahannya diperoleh dari dua angka sebelumnya, contohnya adalah seperti ini 
```java
0, 1, 1, 2, 3, 5, 8, 13, 21, ...dst
```

Yang mana rumus fibonacci berarti sebagai berikut:
```java
fn = (fn-2) + (fn-1)
```

Artinya nilai fn diperoleh dari penjumlahan dua nilai sebelumnya
Deret ini ditemukan pertama kali oleh seorang matematikawan cerdas asal India Gopala Chanda dengan tujuan mencari susunan barang yang tepat untuk dimasukan kedalam kantong  agar distribusi bisa lebih efektif.

Kemudian sorang matematikawan barat yang berasal dari Italia, Leonardo "Fibonacci" Da Pisa (1170-1250,) mengadaptasi dan mengembangkan deret ajaib ini untuk menghitung pola perkembangbiakan kelinci yang ia amati dan tuliskan dalam buku karangannya yang berjudul Liber Abaci. 

Pada awalnya para ilmuwan menganggap remeh pengkajian Fibonacci mengenai deret angka ini karena dianggap hanya sebuah teka-teki matematika saja, Hingga akhirnya pada abad ke-19 Eduard Lucas menyadari berbagai keunikan deret angka ini dan mempelajarinya lebih lanjut.

# Algoritma Deret Fibonacci pada Java

```java
package JavaBasic;
import java.util.*;

public class deretFibonacci{
    public static void main(String[] args) {
        // 0 1 2 3 4 5  6  7   8 dst
        //  1 3 5 7 9 11 13  15
        // rumusnya fn = (fn-1) + (fn-2)

        // ngitung deret fibonacco ke-n
        int f_n, f_n_1, f_n_2, n;

        Scanner inputNilai = new Scanner(System.in);
        
        System.out.print("Masukkan nilai n : ");
        n = inputNilai.nextInt();

        f_n = 0;
        f_n_1 = 1;
        f_n_2 = 0;
        
        for (int i = 0; i <= n; i++ ){ // misal n = 10
            System.out.println("Nilai ke - " + i + " Adalah " + f_n);
            //nilai ke - 0 Adalah 0

            f_n = f_n_1 + f_n_2; // f_n = 1 + 0 = 1
            f_n_2 = f_n_1; // f_n_2 = f_n_1 = 1
            f_n_1 = f_n; // f_n_1 = f_n = 1 
            
            //nilai ke - 1 Adalah 1 
            // f_n = f_n_1 + f_n_2 = 2
            // f_n_2 = f_n_1 = 1
            // f_n_1 = f_n = 2

            // nilai ke - 2 Adalah 2
            // f_n = f_n_1 + f_n_2 = 3
            // f_n_2 = f_n_1 = 2
            // f_n_1 = f_n = 3

            // dst
        }
    }
}
```

<div align="center">
  <a href="https://github.com/falahdrrhmn/Tutorial-Java/blob/main/README.md">(Basic Java)</a>
  
</div>

<br>
<br>

<div align="center">
    Follow me!<br>
    <a href="https://bit.ly/3Qcg3s4">LinkedIn</a>
    ·
    <a href="https://bit.ly/3oRMMaA">Instagram</a>
    ·
    <a href="https://bit.ly/3zqrTrP">Youtube</a>
</div>

