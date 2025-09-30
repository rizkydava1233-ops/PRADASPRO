# Belajar Java – REPORT

## Deskripsi

Dokumen ini merupakan laporan / modul pengenalan dasar bahasa pemrograman **Java**. Java adalah bahasa pemrograman populer yang digunakan untuk membangun aplikasi desktop, web, hingga Android. Report ini menjelaskan instalasi Java, cara menjalankan program pertama, serta contoh kode dasar untuk pemula.

---

## Persiapan / Dependencies

Sebelum memulai, pastikan perangkat mendukung hal berikut:

- **Sistem Operasi**: Windows 10/11 (bisa juga Linux / macOS)
- **Java Development Kit (JDK) versi 8+**
  - Unduh di: https://www.oracle.com/java/technologies/javase-downloads.html
- **IDE / Code Editor (pilih salah satu):**
  - IntelliJ IDEA *(disarankan)*
  - VS Code + Extension Java
  - NetBeans
  - Notepad++ *(jika ingin manual)*

---

## Instalasi Java

1. Unduh file installer **JDK** dari link di atas
2. Install seperti biasa dengan opsi default
3. Cek apakah sudah terpasang dengan membuka **Command Prompt / Terminal**:

```
## Open Terminal jika ingin mengetahui version java telah terinstal

java -version
javac -version
```

Jika versi Java muncul, maka instalasi berhasil.

---

## Menjalankan Program Java Pertama

### 1. Buat File Baru

Buat file dengan nama **HelloWorld.java** dan isi dengan:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, Java!");
    }
}
```

### 2. Compile dan Jalankan

```
javac HelloWorld.java
java HelloWorld
```

**Output:**

```
Hello, Java!
```

---

## Contoh Program Dasar Lain

### Input Output

```java
import java.util.Scanner;

public class InputExample {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.print("Masukkan nama: ");
        String nama = input.nextLine();
        System.out.println("Halo, " + nama + "!");
    }
}
```

### Percabangan (if else)

```java
int nilai = 80;
if (nilai >= 75) {
    System.out.println("Lulus");
} else {
    System.out.println("Tidak Lulus");
}
```

### Perulangan (for)

```java
for(int i = 1; i <= 5; i++) {
    System.out.println("Perulangan ke-" + i);
}
```

## Troubleshooting / Bantuan
|-----------------------------------------------------------------------------------------------------------------------|
|                     MASALAH                            |                              SOLUSI                          |
|--------------------------------------------------------|--------------------------------------------------------------|
| `'javac' is not recognized...`                         | Java belum masuk PATH → reinstall atau setting manual PATCH  |
| Error **"public class ... should be in file ..."**     | Nama file harus sama dengan nama class java                  |
| Compile berhasil tapi tidak bisa dijalankan            | Gunakan `java NamaClass` tanpa `.class`                      |
|-----------------------------------------------------------------------------------------------------------------------|
---

## Penulis

Nama: **[DAVA RIZKY HIDAYATULLAH]**  
Kontak: **[GitHub= https://github.com/rizkydava1233-ops/PRADASPRO.git]**

---

## Versi Dokumen

- **1.0 – Rilis pertama (Dasar Java)**

---

## Referensi

- https://www.w3schools.com/java/
- https://docs.oracle.com/javase/
