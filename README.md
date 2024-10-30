Jelaskan apa yang dimaksud dengan stateless widget dan stateful widget, dan jelaskan perbedaan dari keduanya.
Stateless Widget adalah widget yang mempunyai sifat tidak akan berubah, ketika disebabkan oleh interaksi user maupun variabel dan nilai yang ditemukan. Stateful Widget adalah widget yang mempunyai sifat dinamis. Widget dapat berubah dengan adanya interaksi user maupun variabel dan nilai yang ditemukan.

Sebutkan widget apa saja yang kamu gunakan pada proyek ini dan jelaskan fungsinya.
Icon untuk setiap button agar lebih mudah dipahami, text untuk menampilkan teks, dan snackbar untuk menampilkan pesan sementara ketika di tombol di tekan.

Apa fungsi dari setState()? Jelaskan variabel apa saja yang dapat terdampak dengan fungsi tersebut.
setState() merencanakan suatu pembaruan ke suatu state objek komponen. Ketika state berubah, komponen merespons dengan me-render ulang.

1. State Variable: Hanya variabel state yang didefinisikan dalam this.state di dalam komponen yang akan berubah. State ini biasanya berupa objek, array, atau nilai primitif yang mewakili data internal yang digunakan oleh komponen.

2. Derived UI Elements: Karena React merender ulang UI berdasarkan perubahan state, maka elemen-elemen UI yang bergantung pada nilai state juga akan diperbarui setiap kali setState() dipanggil. Misalnya, jika ada kondisi yang memengaruhi elemen visual berdasarkan state, elemen tersebut akan di-render ulang sesuai nilai state baru.

3. Props-dependent Variables: Jika state yang diubah memengaruhi nilai props yang dikirimkan ke komponen turunannya, komponen-komponen tersebut juga akan menerima props baru sesuai perubahan yang dilakukan di setState().

4. Lifecycle Methods: setState() dapat memicu beberapa metode lifecycle seperti componentDidUpdate() di class component atau efek dalam React hooks (useEffect), sehingga variabel atau proses yang bergantung pada nilai state sebelumnya bisa mengalami pembaruan.


Jelaskan perbedaan antara const dengan final.
final:
1. Variabel final dapat diinisialisasi hanya sekali, biasanya saat deklarasi atau dalam konstruktor.
2. Setelah diinisialisasi, nilai dari variabel final tidak dapat diubah selama waktu runtime program.
3. Nilai dari variabel final dapat dihitung secara dinamis selama waktu runtime, yang berarti Anda dapat menginisialisasinya dengan ekspresi atau fungsi yang dihasilkan saat aplikasi berjalan.

const :
1. Variabel const harus diinisialisasi selama waktu kompilasi, yang berarti nilai-nilai ini harus diketahui sebelum program dijalankan.
2. Nilai dari variabel const harus konstan selama waktu kompilasi dan waktu runtime, yang berarti nilai-nilai ini tidak dapat diubah setelah diinisialisasi.
3. Variabel const biasanya digunakan untuk mendefinisikan konstanta yang tetap nilainya sepanjang eksekusi program.

Jelaskan bagaimana cara kamu mengimplementasikan checklist-checklist di atas.
1. Pertama saya membuat aplikasi flutter 
2. Saya buat widget dan button-button yang diperlukan kemudian memberikan warna 
3. serta menampilkan snack bar di dalam button card sederhana dengan icon