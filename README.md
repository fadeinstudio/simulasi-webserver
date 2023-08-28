# simulasi-webserver
Simulasi Webserver dengan teknologi NodeJS

Webserver ini menggunakan port `80` yang diinstall di VPS; lalu akan dikoneksikan ke port `8080`, yang mana port `8080` akan aktif jika tunnel ssh reverse dari localhost terhubung
berikut perintah saat simulasi => `ssh -NR 8080:localhost:80 root@192.168.1.31 -p 22` dengan simulasi IP VPS adalah `192.168.1.31` dengan port SSH `22`
simulasi sederhana berhasil, apabila ssh tunnel dari localhost mati maka VPS akan mengalihkan ke fungsi => `proxy.on('error', function (err, req, res) {});`
