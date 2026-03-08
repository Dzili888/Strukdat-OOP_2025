# Strukdat-assignment-1

# Object Oriented Programming (OOP)

**Mata Kuliah:** Struktur Data dan Pemrograman Berorientasi Objek  
**Nama:** Muhammad Syadzili Abdul Muhyi  
**NRP:** 5027251030\
**Kelas:** B  

---

## Class & Object
### 1. Class
**Class merupakan Blue print atau cetakan untuk membuat sebuah Object.**

di program kali ini, Class utamanya (*abstract class*) adalah `Mahasiswa`. class utamanya diturunkan menjadi:

- `MahasiswaReguler`
- `MahasiswaBeasiswa`

Contoh:
```java
abstract class Mahasiswa {
    private String nama;
    private String nrp;

    public Mahasiswa() {
        this.nama = "Ucup";
        this.nrp = "5027451045";
    }

    public Mahasiswa(String nama, String nrp) {
        this.nama = nama;
        this.nrp = nrp;
    }

    public abstract double UKT();
}
```

### 2. Object
**Object merupakan hasil/representasi (Instance) dari sebuah class.**

Object yang kita pakai:
- `mhsReguler` (merupakan *object* dari class `MahasiswaReguler`)
- `mhsBeasiswa` (merupakan *object* dari class `MahasiswaBeasiswa`)

Contoh:
```java 
MahasiswaReguler mhsReguler = new MahasiswaReguler("Dzili", "5027251030", 5000000);
MahasiswaBeasiswa mhsBeasiswa = new MahasiswaBeasiswa("Ucup", "5027451045");

//ini buat gunain object untuk manggil method
System.out.println("Tagihan UKT Dzili: Rp " + mhsReguler.UKT());
System.out.println("Tagihan UKT Ucup: Rp " + mhsBeasiswa.UKT());
```

