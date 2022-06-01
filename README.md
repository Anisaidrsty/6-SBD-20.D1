# Tugas 6
**Melakukan Backup dan Restore pada MYSQL**

1. Masuk ke databse nama_nim
<img width="569" alt="image" src="https://user-images.githubusercontent.com/101643559/171304914-1c0763e8-501c-467d-9bd3-651392272261.png">

2. Lakukan proses backup dan recovery dengan sql dari database tugas seblumnya !
<img width="746" alt="image" src="https://user-images.githubusercontent.com/101643559/171305238-f329a626-46da-4bde-a9e8-c1a61e049b94.png">

Jika proses backup berhasil maka akan muncul file backuppada direktori C:\xampp\mysql\data\nama database Recovery

<img width="442" alt="image" src="https://user-images.githubusercontent.com/101643559/171305337-bc96fc9b-dd5c-4959-adaf-3d0aef683955.png">

Data yang telah di-backup dapat dikembalikan kapan saja bila diperlukan. Sintaks SQL yang digunakan adalah LOAD DATA INFILE. Perintah yang dijalankan adalah _LOAD DATA INFILE ‘Nama_backup_file’ INTO TABLE nama_table ;_
<img width="780" alt="image" src="https://user-images.githubusercontent.com/101643559/171305707-cd56d110-736c-459d-8b47-eb4eea7cbc76.png">

3. Lakukan proses backup dan recovery dengan sqldump dari database tugas seblumnya !
<img width="811" alt="image" src="https://user-images.githubusercontent.com/101643559/171306202-bba9a624-1338-4f9d-8f2b-208b637b36a1.png">

4. Tulisakan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam !

0 0 * * 0 mysqldump -u root -p anisa_312010040>anisa_312010040_backup.sql


