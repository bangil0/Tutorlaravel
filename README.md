Langkah pengerjaan
Download Source Code dari repo Github Silsilah dalam bentuk Zip.
Extract file zip (source code) ke dalam direktori htdocs pada XAMPP, misal htdocs/web.
Melalui terminal, cd ke direktori web.
(Sesuai petunjuk installasi) Pada terminal, berikan perintah composer install. Ini yang perlu koneksi internet.
Composer akan menginstall dependency paket dari source code tersebut hingga selesai.
Jalankan perintah php artisan, untuk menguji apakah perintah artisan Laravel bekerja.
Buat database baru (kosong) pada mysql (via phpmyadmin).
Duplikat file .env.example, lalu rename menjadi .env.
Kembali ke terminal, php artisan key:generate.
Setting koneksi database di file .env (DB_DATABASE, DB_USERNAME, DB_PASSWORD).
Jalan kan perintah php artisan migrate Jika di cek di phpmyadmin, seharusnya tabel sudah muncul.
Setelah selesai, buka aplikasi melalui browser, misal : http://localhost/web/public
Klik link Register untuk mendaftarkan user baru.
Login dan aplikasi siap digunakan.

Sistem Requirements
PHP >= 7.0.0
MySQL >= 5.7
Local Instalation DEV
Clone from Bitbucket
seting up .env dan database
Run composer install
Run php artisan key:generate
Run php artisan migrate
Run php artisan db:seed
Run php artisan storage:link
Membersihkan pengaturan
Run php artisan config:cache
Jika Bermain Dengan VUE
Run npm install
Run npm run dev / npm run watch / npm run prod
Jika di Server
Run git init
Run git remote add origin https:///rkpd-online.git
Run git pull origin master
Run chown -R nginx:root /var/www/laravel
Run chmod 755 /var/www/laravel/storage
Backup Database di Server
Run cd /home/rkpdonline/backup/sql/
Run mysqldump -u root -p rkpdonline_db > bac_rkpdonline_db_$(date +\%d_\%m_\%Y_\%H_\%M_\%S).sql
Package
Larave Permission
Active for Laravel
