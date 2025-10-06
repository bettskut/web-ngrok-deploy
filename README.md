# web-ngrok-deploy
A simple web project with deployment using Ngrok
## Deployment Steps

1. Install Ngrok:
```bash
sudo snap install ngrok
```
2. Tambahkan Authtoken:
```bash
ngrok config add-authtoken <TOKEN>
```
3. Install Apache2:
```bash
sudo apt install apache2
```
4. Buat file index.html:
```bash
sudo nano /var/www/html/index.html
```
5. Cek apakah sudah berjalan secara lokal:
```bash
curl -I http://localhost

# Harus dapat HTTP/1.1 200 OK
```
6. Jalankan Tunnel Ngrok:
```bash
ngrok http 80

# Jika berhasil maka terminal akan menampilkan URL:
Forwarding https://xxxx-xxxx-xxxx.ngrok-free.app -> http://localhost:80
```
