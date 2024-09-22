CISCO PACKET TRACER

Configurasi router 1:

Untuk memulai konfigurasi pada router kita bisa turn on router di tab physical. Setelah itu menuju cli.
Terdapat 4 layer exec command di router

1. User exec command
   enable => masuk ke Prefillage exec command, akan diminta input password pika sudah men setting password di Global configuration mode
2. Prefillage exec command
   configure terminal => mask ke Global configuration mode
   show running-config => menampilkan konfigurasi stat ini yang dishpan di RAM dan bersifat sementara
   show startup-config => menampilkan konfigurasi stat ini yang dishpan di storage dan bersifat permanen
   copy running-config startup-config => copy konfigurasi dari running-config ke startup-config
   banner motd &[message]& => setting message ketika router booting
3. Global configuration mode
   enable password [password] => setting password plain text
   enable secret [password] => setting password dengan enkripsi (akan mengganti password existing)
   hostname [nama router] => setting nama router
   line console 0 >> password [password] >> login => setting password mask ke user exec

Interface configuration mode
