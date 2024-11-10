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
