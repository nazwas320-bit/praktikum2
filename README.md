latihan1.py

# 🧮 Program Mencari Bilangan Terbesar dari 4 Bilangan (Python)

Program ini dibuat untuk **menentukan bilangan terbesar dari empat bilangan** yang dimasukkan oleh pengguna menggunakan **statement `if`** dalam bahasa pemrograman **Python**.

---

## 📘 Deskripsi Program

Program akan meminta pengguna untuk memasukkan **4 bilangan**, kemudian menggunakan logika **percabangan `if`** untuk menentukan bilangan mana yang paling besar.

Setelah itu, hasil akan ditampilkan di layar beserta bilangan yang dimasukkan.

---

## 💡 Fitur Program

- Input 4 bilangan dari pengguna.  
- Menentukan bilangan terbesar menggunakan kondisi `if`.  
- Menampilkan hasil dengan format yang rapi.

---

## 🧾 Contoh Kode Program

```python
# Program Mencari Bilangan Terbesar dari 4 Bilangan
# Menggunakan Statement IF

print("=" * 24)
print("PROGRAM MENCARI BILANGAN TERBESAR")
print("=" * 24)

# Input 4 buah bilangan
bil1 = float(input("Masukkan bilangan ke-1: "))
bil2 = float(input("Masukkan bilangan ke-2: "))
bil3 = float(input("Masukkan bilangan ke-3: "))
bil4 = float(input("Masukkan bilangan ke-4: "))

# Menentukan bilangan terbesar menggunakan if
terbesar = bil1  # Anggap bil1 adalah yang terbesar

if bil2 > terbesar:
    terbesar = bil2

if bil3 > terbesar:
    terbesar = bil3

if bil4 > terbesar:
    terbesar = bil4

# Menampilkan hasil
print("\n" + "=" * 24)
print(f"Bilangan yang Anda masukkan: {bil1}, {bil2}, {bil3}, {bil4}")
print(f"Bilangan TERBESAR adalah: {terbesar}")
print("=" * 24)

latihan2.py


# 🔢 Program Mengurutkan Data dari Terkecil ke Terbesar (Python)

Program ini digunakan untuk **mengurutkan sekumpulan data numerik** berdasarkan input pengguna dari **yang terkecil ke terbesar**.  
Program dibuat menggunakan bahasa **Python** dengan logika dasar `if`, `for`, dan metode `sort()` pada list.

---

## 📘 Deskripsi Program

Pengguna diminta memasukkan sejumlah data (minimal 2).  
Semua data disimpan dalam list, kemudian diurutkan menggunakan fungsi bawaan Python `sort()`.  
Hasil akhirnya menampilkan urutan data dari yang **terkecil hingga terbesar**.

---

## 💻 Kode Program

```python
# program mengurutkan data dari terkecil ke terbesar

print(" program pengurutan data ")

# meminta jumlah data 
jumlah = int(input("masukkan jumlah data (minimal 2): "))

if jumlah < 2: 
     print("jumlah data harus minimal 2!")
else:
    data = []
    # input data sebanyak jumlah yang diminta 
    for i in range(jumlah):
        nilai = int(input(f"masukkan data ke-{i+1}: "))
        data.append(nilai)
    # mengurutkan data dari kecil ke besar 
    data.sort()
    # menampilkan hasil
    print("\ndata setelah diurutkan (dari terkecil ke terbesar):")
    for d in data:
        print(d)
```

---

## 🧠 Penjelasan Program

1. **Input jumlah data**  
   Pengguna menentukan berapa banyak data yang ingin diurutkan.
   ```python
   jumlah = int(input("masukkan jumlah data (minimal 2): "))
   ```

2. **Validasi jumlah data**  
   Program memastikan jumlah data minimal dua.
   ```python
   if jumlah < 2:
       print("jumlah data harus minimal 2!")
   ```

3. **Input data satu per satu**  
   Menggunakan perulangan `for` untuk mengisi list `data`.
   ```python
   for i in range(jumlah):
       nilai = int(input(f"masukkan data ke-{i+1}: "))
       data.append(nilai)
   ```

4. **Mengurutkan data**  
   Menggunakan fungsi bawaan `sort()` untuk mengurutkan list.
   ```python
   data.sort()
   ```

5. **Menampilkan hasil**  
   Hasil pengurutan ditampilkan satu per satu dengan perulangan.
   ```python
   for d in data:
       print(d)
   ```

---

## 📊 Contoh Hasil Eksekusi

```
 program pengurutan data 
masukkan jumlah data (minimal 2): 5
masukkan data ke-1: 10
masukkan data ke-2: 3
masukkan data ke-3: 7
masukkan data ke-4: 1
masukkan data ke-5: 9

data setelah diurutkan (dari terkecil ke terbesar):
1
3
7
9
10
```

---

## 🧩 Fitur Tambahan yang Bisa Dikembangkan

- Mengurutkan dari **terbesar ke terkecil** (`data.sort(reverse=True)`).
- Mengurutkan **angka desimal (float)**.
- Menampilkan **rata-rata, nilai minimum, dan maksimum** dari data.

---

