# Strukdat-assignment-1

# Object Oriented Programming (OOP)

**Mata Kuliah:** Struktur Data dan Pemrograman Berorientasi Objek  
**Nama:** Muhammad Syadzili Abdul Muhyi  
**NRP:** 5027251030\
**Kelas:** B  

---

## 1. Class & Object

### Class
Di tugas kali ini, aku pakai struktur di mana `Mahasiswa` bertindak sebagai *abstract class* (induk). Dari induk ini, diturunkan lagi menjadi dua *class* spesifik:
- `MahasiswaReguler`
- `MahasiswaBeasiswa`

Berikut adalah cuplikan *source code* untuk class utamanya:
```java
abstract class Mahasiswa {
    private String nama;
    private String nrp;

    public Mahasiswa() {
        this.nama = "Belum diisi";
        this.nrp = "0000000";
    }

    public Mahasiswa(String nama, String nrp) {
        this.nama = nama;
        this.nrp = nrp;
    }

    public abstract double hitungNilaiAkhir();
}