# Tugas-Praktikum-4
### program sederhana untuk menambahkan data kedalam sebuah list
1. Variable baru, nilai variablenya diisi dengan '[]'
###
    Datat = []

2. Membuat Perulangan (While loop) dan Variable baru dengan nilai yang akan menerima jawaban (ya/tidak) secara berulang kali. Jika Data = 'y', maka x = 0 (loop akan terus berlanjut). Jika Data = 'n', maka x = 1 (loop akan berhenti)
###
    Datat = []
    x = 0
    
    while x == 0
      Data = input("Tambah Data? (Y/N)")
      if Data == 'y' or Data == 'Y':
        x = 0
      elif Data == 'n' or Data == 'N':
        x = 1
3. Variable indeks untuk menambahkan list/user dari data diinput. Pada saat Data = 'y', Indeks tersebut akan ditambah dengan 1 untuk mengisi data, bagaian, atau user yang tepat
###
    while x == 0:

      if Data == 'y' or Data == 'Y':
        index = index + 1
        Datat.insert(index,[])
        
      Data = input("Tambah Data? (Y/N)")
      if Data == 'y' or Data == 'Y':
        x = 0
      elif Data == 'n' or Data == 'N':
        x = 1
4. Fungsi input() untuk mengambil data Nama, NIM, Tugas, UTS, UAS, dan Nilai Akhir. Gunakan fungsi 'append' untuk mengirim Data A yang sudah diisi ke data B (Datat = []).
###
    Datat = []
    index = -1
    Data = "y"
    x = 0
    while x == 0:
      if Data == 'y' or Data == 'Y':
        index = index + 1
        Datat.insert(index,[])

        while True:
            Nama = Datat[index].append(input("Nama : "))
            Nim = Datat[index].append(input("NIM : "))

            Tugas = int(input("Tugas : "))
            Datat[index].append(Tugas)

            UTS = int(input("UTS : "))
            Datat[index].append(UTS)

            UAS = int(input("UAS : "))
            Datat[index].append(UAS)

            akhir = Tugas * 0.3 + UTS * 0.35 + UAS * 0.35
            Datat[index].append(akhir)
            break
      Data = input("Tambah Data? (Y/N)")
      if Data == 'y' or Data == 'Y':
        x = 0
      elif Data == 'n' or Data == 'N':
        x = 1
5. Jika x = 1 atau variable Data mendapatkan nilai 'n' (tidak), loop akan ditutup dan melompati ke bagian hasil (x == 1)
###
    if x == 1:
      print("==============================================================")
      print("| No |  Nama   |    NIM    | Tugas | UTS | UAS | Akhir |")
      print("==============================================================")
6. Gunakan for loop pada Data list
###
    if x == 1:
      print("==============================================================")
      print("| No |  Nama   |    NIM    | Tugas | UTS | UAS | Akhir |")
      for i in range(len(Datat)):
        print(f"| {i + 1}  | {Datat[i][0]} | {Datat[i][1]} |  {Datat[i][2]}  | {Datat[i][3]}  | {Datat[i][4]}  | {Datat[i][5]}  |")
      print("==============================================================")
![image](https://user-images.githubusercontent.com/61907877/143869842-ca116b9e-39a5-4e87-be8a-56c41a194c15.png)
![Flowchartt (1)](https://user-images.githubusercontent.com/61907877/143875776-f7beea12-2f33-43be-8e7a-81824195b469.png)


