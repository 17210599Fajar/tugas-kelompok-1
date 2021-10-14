nim = input("Masukan NIM = ")
nama = input("Masukan Nama = ")
kelas = input("Masukan Kelas = ")
matkul = input("Masukan Matakuliah = ")
nilai_absen = int(input("Nilai Absen = "))
nilai_tugas1 = int(input("Nilai Tugas 1 = "))
nilai_tugas2 = int(input("Nilai Tugas 2 = "))
nilai_uts = int(input("Nilai UTS = "))
nilai_uas = int(input("Nilai UAS = "))


# prosses

any = nilai_absen * 0.20 + nilai_tugas1 * 0.10 + \
    nilai_tugas2 * 0.10 + nilai_uts * 0.30 + nilai_uas * 0.30


# output

print("=======================================")
print("NIM      :"+str(nim))
print("NAMA     :"+str(nama))
print("KELAS    :"+str(kelas))
print("MATKUL   :"+str(matkul))

if any >= 85:
    print("GRADE A")
    print("SELAMAT NILAI ANDA SANGAT BAGUS DAN ANDA LULUS")

elif any >= 75:
    print("GRADE B")
    print("SELAMAT NILAI ANDA CUKUP BAGUS DAN ANDA LULUS")

elif any >= 65:
    print("GRADE C")
    print("SELAMAT NILAI ANDA CUKUP DAN ANDA LULUS")

else:
    print("GRADE D")
    print("NILAI ANDA BELUM CUKUP DAN ANDA BELUM LULUS")

print("TOTAL NILAI KESELURUHAN = "+str(any))
print("=======================================")
