Question : 

![](https://github.com/MrPayMac/picoCTF/blob/main/Forensic/Matryoshka%20doll/Question.png)

Hint :

![](https://github.com/MrPayMac/picoCTF/blob/main/Forensic/Matryoshka%20doll/Hints1.png)
di hint tersebut menjelaskan bahwa ada file tersembunyi di dalam file


1. gunakan `binwalk dolls.jpg` untuk melihat apakah ada file tersembunyi di dalam gambar tersebut

![](https://github.com/MrPayMac/picoCTF/blob/main/Forensic/Matryoshka%20doll/binwalk.png)
terlihat bahwa terdapat 2 file di dalam nya, yaitu file zip dan folder base_images yang didalam folder tersebut terdapat file 2_c.jpg

2. ketik `binwalk -e dolls.jpg` untuk mengekstrak gambar tersebut

3. Lalu masuk ke dalam folder yang telah di ekstrak, biasanya berawalan '_'
   
4. masuk ke folder base_images, ketika tidak menemukan flag nya dan hanya terdapat file jpg saja. ketik `binwalk (file.jpg)` untuk mengecek apakah file jpg tersebut memiliki file tersembunyi di dalam nya
5. ketika sudah di ekstrak dan masih belum menemukan. cobalah untuk mengestraknya terus menerus sampai menemukan flag nya

flag = `picoCTF{bf6acf878dcbd752f4721e41b1b1b66b}`


