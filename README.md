# 🌍 GeoServer Config

Repository ini berisi konfigurasi dan panduan instalasi **GeoServer 2.26.2** pada **WSL2** dengan **JRE 11**.

---

## 🛠 Persyaratan
Sebelum memulai instalasi, pastikan Anda memiliki:
✅ **WSL2** (Windows Subsystem for Linux 2)  
✅ **Ubuntu 20.04+**  
✅ **JRE 11** (OpenJDK atau AdoptOpenJDK)  
✅ **GeoServer 2.26.2**  

---

## 🚀 Instalasi GeoServer

### 1️⃣ Perbarui Sistem dan Instal Java 11
Jalankan perintah berikut untuk memastikan sistem Anda diperbarui dan Java 11 terinstal:
```sh
sudo apt update && sudo apt upgrade -y
sudo apt install openjdk-11-jre unzip wget -y
```

Cek versi Java untuk memastikan:
```sh
java -version
```
Pastikan output menunjukkan **Java 11**.

---

### 2️⃣ Unduh dan Ekstrak GeoServer
Unduh GeoServer 2.26.2 dari sumber resmi:
```sh
wget https://sourceforge.net/projects/geoserver/files/GeoServer/2.26.2/geoserver-2.26.2-bin.zip
unzip geoserver-2.26.2-bin.zip
mv geoserver-2.26.2 ~/geoserver
```

---

### 3️⃣ Jalankan GeoServer
Masuk ke folder GeoServer dan jalankan server:
```sh
cd ~/geoserver/bin
./startup.sh
```

GeoServer sekarang berjalan di **`http://localhost:8080/geoserver`** 🎉

---

## ⚙️ Konfigurasi Tambahan
📂 **Data Directory**: Semua konfigurasi disimpan di `~/geoserver/data_dir`  
🔑 **User Default**:  
   - **Username**: `admin`  
   - **Password**: `geoserver`  
📝 **Logging**: File log dapat ditemukan di `~/geoserver/data_dir/logs/geoserver.log`

---

