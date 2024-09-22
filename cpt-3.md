# Membuat Arsitektur jaringan 1 router, 2 switch, 4 pc

1. Menambah 4 pc dengan 2 switch masing-masing switch 2 pc.
2. Config Ip pada pc dengan subnet 255.255.255.0
    a. 192.168.1.0 => 192.168.1.1 dan 192.168.1.2
    b. 192.168.2.0 => 192.168.2.1 dan 192.168.2.2
3. Sambungkan dengan switch

    ![This is an alt text.](/connect-pc-switch.png "connect-pc-switch")

4. Sambung kedua switch dengan router 
    - ip 192.168.1.0 ke interface fa0/0
    - ip 192.168.2.0 ke interface fa1/0

    ![This is an alt text.](/connect-switch-router.png "connect-switch-router")

5. Passang ip pada masing masing interface dengan command di router
    - ```interface fa0/0``` pada global-configuration-mode 
    - tambah ip address dengan command ```ip address 192.168.1.254```

    ![This is an alt text.](/tambah-ip-interface.png "tambah-ip-interface")

6. Lakukan uji koneksi melalui pc to router / router to pc
7. Psang gateway pada masing-masing pc sesuai ip interface agar pc bisa connect ke pc lain yang berbeda ip atau interface tetapi masih dalam satu router.

    ![This is an alt text.](/pasang-gateway.png "pasang-gateway")