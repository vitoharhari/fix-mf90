# fix-mf90
- Fix mf90 bypass not power on if stb hg680p openwrt reboot

- script hg680p.sh by Lutfailham96.
Visit github Lutfailham96 on : https://github.com/lutfailham96

- Cara pakai :

Copy dan paste kan perintah ini di stb hg680p openwrt anda

- Perintah pertama : 

wget --no-check-certificate "https://raw.githubusercontent.com/vitoharhari/fix-mf90/main/hg680p.sh" -O /usr/bin/hg680p.sh && chmod +x /usr/bin/hg680p.sh

- Perintah kedua : 

wget --no-check-certificate "https://raw.githubusercontent.com/vitoharhari/fix-mf90/main/autorebootmifi.sh" -O /root/autorebootmifi.sh && chmod +x /root/autorebootmifi.sh

- Lalu masukkan perintah berikut ini kedalam rc.local (local startup)

#!/bin/bash
/root/autorebootmifi.sh
exit 0

- Setelah itu save dan tes dengan reboot stb hg680p openwrt anda
