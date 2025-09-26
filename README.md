
1. File .sh tidak bisa dieksekusi, bisa ditulis seperti  izin:
```
chmod +x namafile.sh
```
Lalu jalankan:
```
./namafile.sh
```
___

2. Perbaiki Format File

Jika script dibuat di Windows, bisa muncul error karakter ^M.
Gunakan perintah berikut untuk memperbaiki:
```
sed -i 's/\r$//' namafile.sh
```
atau
```
dos2unix namafile.sh
```

---

3. Jalankan dengan Interpreter

Jika tetap tidak bisa, jalankan langsung dengan:
```
bash namafile.sh
```
atau
```
./namafile.sh
```


