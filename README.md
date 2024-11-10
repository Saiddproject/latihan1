# latihan1
Input Pengguna: Program meminta pengguna untuk memasukkan nilai n, yaitu jumlah bilangan acak yang ingin ditampilkan. Nilai n ini diinputkan pada runtime.

Proses: Program menggunakan perulangan while untuk memastikan jumlah bilangan acak yang dihasilkan dan ditampilkan sesuai dengan yang diminta oleh pengguna. Setiap bilangan acak dihasilkan menggunakan random.random(), yang menghasilkan bilangan acak antara 0 dan 1. Jika bilangan acak yang dihasilkan lebih kecil dari 0.5, maka bilangan tersebut akan ditampilkan. Proses ini akan terus berlanjut sampai jumlah bilangan yang ditampilkan mencapai nilai n.

Output: Program akan menampilkan sejumlah bilangan acak yang lebih kecil dari 0.5 sesuai dengan jumlah yang diminta oleh pengguna.

    # Meminta input dari pengguna untuk jumlah bilangan acak yang ingin ditampilkan
    n = int(input("Masukkan jumlah bilangan acak yang ingin ditampilkan: "))

    # Meminta input dari pengguna untuk jumlah bilangan acak yang ingin ditampilkan
    n = int(input("Masukkan jumlah bilangan acak yang ingin ditampilkan: "))
    count = 0  # Variabel untuk menghitung jumlah bilangan acak yang telah ditampilkan
    
    # Menggunakan while loop untuk terus menampilkan bilangan acak sampai mencapai jumlah yang diinginkan
    while count < n:
        # Menghasilkan bilangan acak antara 0 dan 1
        random_number = random.random()
        
        # Jika bilangan acak lebih kecil dari 0.5, tampilkan
        if random_number < 0.5:
            print(random_number)
            count += 1  # Menambah hitungan bilangan yang sudah ditampilkan
            
# latihan2
Modal Awal: 
Program mulai dengan modal usaha sebesar 100 juta.

Proses:
Program menggunakan perulangan for untuk menghitung keuntungan bulan demi bulan selama 8 bulan.
Keuntungan pada setiap bulan dihitung dengan persentase yang berbeda:
Bulan 1 dan 2: Tidak ada keuntungan (0%).
Bulan 3: Keuntungan 1% dari modal awal.
Bulan 5: Keuntungan meningkat menjadi 5% dari modal awal.
Bulan 8: Keuntungan menurun menjadi 3% dari modal awal.
Bulan lainnya: Keuntungan tetap 1%.
Keuntungan setiap bulan akan ditambahkan ke total keuntungan yang dihitung.

Output:
Program menampilkan total keuntungan yang diperoleh setelah 8 bulan berjalan, dalam format mata uang yang mudah dibaca
    
    # Modal awal usaha (dalam juta rupiah)
    modal_awal = 100000000  # 100 juta
    keuntungan = 0  # Inisialisasi total keuntungan
     # Loop selama 8 bulan
    for bulan in range(1, 9):
        # Kondisi keuntungan berdasarkan bulan
        if bulan == 1 or bulan == 2:
            # Pada bulan 1 dan 2 tidak ada keuntungan
            laba_bulan = 0
        elif bulan == 3:
            # Pada bulan 3, laba mulai 1% dari modal awal
            laba_bulan = 0.01 * modal_awal
        elif bulan == 5:
            # Pada bulan 5, laba meningkat menjadi 5%
            laba_bulan = 0.05 * modal_awal
        elif bulan == 8:
            # Pada bulan 8, laba menurun menjadi 3%
            laba_bulan = 0.03 * modal_awal
        else:
            # Untuk bulan selain yang disebutkan, laba tetap 1%
            laba_bulan = 0.01 * modal_awal
        
        # Menambahkan keuntungan bulan ini ke total keuntungan
        keuntungan += laba_bulan  

    # Menampilkan total keuntungan selama 8 bulan
    print(f"Total keuntungan selama 8 bulan adalah: Rp {keuntungan:,.2f}")

# latihan3
