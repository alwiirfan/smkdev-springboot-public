# Apa itu OpenJDK?

---

> OpenJDK (Open Java Development Kit) adalah implementasi open-source dari platform Java Standard Edition (Java SE). Ini adalah proyek yang dikembangkan oleh komunitas dengan kontribusi utama dari Oracle Corporation. OpenJDK menyediakan lingkungan runtime Java, perpustakaan standar, dan alat pengembangan seperti compiler Java (javac).

---

# Instalasi Java

Sebelum Belajar bahasa pemrograman Java yang dilakukan pertama kali yaitu menginstall Java di Komputer yang kita pakai. Java dapat di install di semua sistem Operasi baik Linux, Windows maupun MacOS.

## **Linux**

> Berikut adalah cara instalasi OpenJDK 17 atau Java 17 di sistem operasi Linux.
> **Catatan:** Cara ini bisa di gunakan untuk install Java versi berapapun sesuai OpenJDK yang kita unduh.

---

Berikut proses untuk instalasi Java pada Linux:

1. Kunjungi situs resmi `OpenJDK` di [https://jdk.java.net/archive/](https://jdk.java.net/archive/) untuk mengunduh file instalasi Java yang sesuai dengan arsitektur sistem operasi Linux kamu (misalnya amd64, untuk arsitektur 64-bit).
2. Buka terminal pada Linux:

- Buat directory terlebih dahulu untuk menyimpan file Java yang akan di extract:

```bash
mkdir /opt/openjdk
```

- Masuk ke Downloads dengan melakukan perintah:

```bash
cd Downloads/
```

3. Extract file yang telah di unduh, dengan perintah berikut (file yang telah di unduh `openjdk-17.0.2_linux-x64_bin.tar.gz`):

```bash
tar -zxf openjdk-17.0.2_linux-x64_bin.tar.gz -C /opt/openjdk
```

---

4. Masuk ke shell yang kita gunakan (contoh: dengan menggunakan `.bashrc`):

```bash
nano ~/.bashrc
```

- Tambahkan `JAVAHOME`:

```bash
export JAVA_HOME="/opt/openjdk/jdk-17.0.2"
export PATH="$JAVA_HOME/bin:$PATH"
```

- Lalu simpan perubahan yang telah di tambahkan.

---

5. Tutup terminal dan buka terminal baru:

- Cek apakah Java 17 sudah terinstall, dengan melakukan perintah:

```bash
java --version
```

- _Output:_

```bash
openjdk 17.0.2 2022-01-18
OpenJDK Runtime Environment (build 17.0.2+8-86)
OpenJDK 64-Bit Server VM (build 17.0.2+8-86, mixed mode, sharing)
```

- Cek Java Compiler (javac):

```bash
javac --version
```

- _Output:_

```bash
javac 17.0.2
```

---
