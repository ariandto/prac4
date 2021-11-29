<p align="center">
Membuat Data Mahasiswa Menggunakan List dan Perulangan
</p>
<p>

A. Penjelasan Program Latihan 1#<p>
a. FlowChart<p>
<p align="center">
<img src="https://github.com/ariandto/prac4/blob/main/pct/hs0.png"/>
<p align="center">
</p>

Source Code:</p>

```python
data=[]
while True:
    nama=input("Nama Mahasiswa\t: ")
    nim=input("NIM\t\t: ")
    tugas=int(input("Nilai Tugas\t: "))
    uts=int(input("Nilai UTS\t: "))
    uas=int(input("Nilai UAS\t: "))
    na=(int(tugas)*.30)+(int(uts)*.35)+(int(uas)*.35)
    data.append([nama,nim,tugas,uts,uas,na])
    
    lanjut=input("tambah data??(y/t)")
    if lanjut=="t" or lanjut=="T":
        print("data mahasiswa")
        print("=================================================================================================")
        print("|\tNAMA\t|\tNIM\t|\tTUGAS\t|\tUTS\t|\tUAS\t|\tAKHIR\t|")
        print("=================================================================================================")
        for x in data:
            print("\t{0:1}\t|\t{1:1}\t|\t{2:1}\t|\t{3:1}\t|\t{4:1}\t|\t{5:1}\t|".format(x[0],x[1],x[2],x[3],x[4],x[5]))
            print("=================================================================================================")
        else:
            break
```
Hasil Program sebagai berikut<p>
<p align="center">
<img src="https://github.com/ariandto/prac4/blob/main/pct/hs1.png"/>
<p align="center">
</p>


Keterangan</p>

```python
while True:
```
- Berarti loop selamanya. Pernyataan mengambil ekspresi dan mengeksekusi tubuh loop sementara mengevaluasi ekspresi (boolean) "benar". True selalu mengevaluasi ke boolean "true" dan dengan demikian mengeksekusi badan perulangan tanpa batas.<p>
