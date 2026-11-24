# 1. Definisi Class Cafe
 class Cafe:
     nama = ""
     alamat = ""
 # 2. Definisi Class Orang
 class Orang:
CODING PYTHON DAN OUTPUT
Percakapan Alam dan Budi di Kafe Kopi Kenangan Senja
    nama = ""
    nim = 0  # Instance attribute untuk NIM
    # Method untuk menyapa/berkenalan
    def perkenalan(self):
        print(f"Halo, nama saya {self.nama} (NIM: {self.nim}).")
    # Method untuk menyapa orang lain
    def hello(self, nama_lawan_bicara):
        print(f"Halo {nama_lawan_bicara}, nama saya {self.nama} (NIM: {self.nim}).")
    # Method khusus percakapan di kafe
    def pesan_kopi(self, pesanan):
        print(f"{self.nama}: Saya pesan {pesanan} ya.")
# ==========================================
# IMPLEMENTASI DAN PERCAKAPAN
# ==========================================
# Instansiasi Object Cafe
kafe1 = Cafe()
kafe1.nama = "Kopi Kenangan Senja"
kafe1.alamat = "Jl. Sudirman No. 45, Jakarta Pusat"
# Instansiasi Object Orang (Alam dan Budi) dengan NIM baru
orang1 = Orang()
orang1.nama = "Alam"
orang1.nim = 14022500137
orang2 = Orang()
orang2.nama = "Budi"
orang2.nim = 14022500000
# --- Buka Percakapan ---
print("=" * 60)
print(f"LOKASI: {kafe1.nama}")
print(f"ALAMAT: {kafe1.alamat}")
print("=" * 60)
print("\n--- Awal Pertemuan di Kafe ---\n")
# Budi menyapa Alam duluan
orang2.hello(orang1.nama)
# Alam membalas perkenalan
orang1.perkenalan()
# Percakapan berlanjut mengenai pesanan
print()
orang1.pesan_kopi("Americano Ice")
orang2.pesan_kopi("Hazelnut Latte")
print("\nAlam: Boleh saya duduk di meja ini?")
print("Budi: Tentu, silakan duduk!")
print("=" * 60)
