<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./images/3xui.png">
    <img alt="3x-ui" src="./images/3xui.png">
  </picture>
</p>


## Install & Upgrade

```
sudo apt update && sudo apt upgrade -y
```

## Install & Upgrade

```
bash <(curl -Ls https://raw.githubusercontent.com/mhsanaei/3x-ui/master/install.sh)
```

## To ensure proper access, configure your firewall with the following commands
```
sudo ufw allow 1024:65535/tcp
sudo ufw allow 443/tcp
sudo ufw allow 80/tcp
sudo ufw enable
sudo ufw allow 8080
```

## SSL Certificate

To install and use Certbot:

```sh
apt-get install certbot -y
sudo certbot certonly --standalone -d yourdomain.com -d www.yourdomain.com
certbot renew --dry-run
```

Without-WWW. :

```sh
sudo certbot certonly --standalone -d yourdomain.com
certbot renew --dry-run
```

Without-Email:

```sh
certbot certonly --standalone --agree-tos --register-unsafely-without-email -d yourdomain.com
certbot renew --dry-run
```

SSL Domain Expire Date စစ်ရန် :

```sh
certbot certificates
```

Domain Certificate ကိုဖျက်မယ် :

```sh
sudo certbot delete
```

အပိုဖိုင်များကို ဖျက်ရန် (Optional) :

```sh
sudo rm -rf /etc/letsencrypt/live/yourdomain.com
sudo rm -rf /etc/letsencrypt/archive/yourdomain.com
sudo rm -rf /etc/letsencrypt/renewal/yourdomain.com.conf
```

## Reverse Proxy URI (Optional)

```
https://orgpg.shop/v2/api-secure/8Hs9X2T/
```

### **Clone the Project Repository:**

   ```sh
   git clone https://github.com/MHSanaei/3x-ui.git
   cd 3x-ui
   ```

## Recommended OS

- Ubuntu 20.04+
- Debian 11+
- CentOS 8+
- OpenEuler 22.03+
- Fedora 36+
- Arch Linux
- Parch Linux
- Manjaro
- Armbian
- AlmaLinux 8.0+
- Rocky Linux 8+
- Oracle Linux 8+
- OpenSUSE Tubleweed
- Amazon Linux 2023
- Windows x64

ed with early embedded systems, it is less common today but may still be found in legacy devices like early Raspberry Pi versions and some older smartphones.

- **s390x**: This architecture is commonly used in IBM mainframe computers and offers high performance and reliability for enterprise workloads.
