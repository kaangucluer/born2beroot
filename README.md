>> URL : https://kindhearted-stem-72f.notion.site/Born2beroot-b41fa96d65b740b6b7a46ed53a57a2c8


>> ***Signature.txt ve born2beroot.vdi Dosyasının karşılaştırıması***

- Terminal > cd goinfree > cd born2beroot > shasum born2beroot.vdi

>> ***********************************************Sanal Makina Nasıl Çalışır ?***********************************************

- Sanal makine, bir işletim sistemini fiziksel bir bilgisayarın donanımından izole eden bir yazılım uygulamasıdır. Sanal makineler, birden fazla işletim sistemini aynı fiziksel bilgisayarda çalıştırmak, farklı işletim sistemlerini test etmek ve geliştirmek ve farklı yazılımları çalıştırmak için kullanılabilir.
- Sanal makineler, bir hipervizör adı verilen bir yazılım tarafından yönetilir. Hipervizör, fiziksel bilgisayarın donanımını sanal makineler arasında dağıtır. Her sanal makine, kendi işlemci, bellek, depolama ve ağ kaynaklarına sahiptir.

>> ***Rock ve Debian arasındaki temel farklar nelerdir ?***

- Rocky Linux, Debian'dan daha az paket içerir, bu da Rocky Linux'un daha hafif ve daha hızlı olduğu anlamına gelir.
- Rocky Linux, Debian'dan daha yeni bir işletim sistemidir, bu da Rocky Linux'un daha yeni özellikler ve güvenlik güncellemelerine sahip olduğu anlamına gelir.
- Rocky Linux, CentOS Stream'den geliştirilmişken, Debian, 30 yılı aşkın süredir var olan ve Linux dünyasında tanınmış bir isim olan daha eski bir işletim sistemidir.
- Rocky Linux, Debian'dan daha kurumsal odaklı bir işletim sistemidir. Rocky Linux, Debian'dan daha uzun destek sürelerine ve daha iyi güvenlik özelliklerine sahiptir.
- Genel olarak, Rocky Linux, daha yeni, daha hızlı, daha kurumsal odaklı bir işletim sistemidir. Debian, daha eski, daha hafif, daha ev kullanıcısı odaklı bir işletim sistemidir.

*****************************************************>> Sanal Makinelerin Amacı nedir ?*****************************************************

- birden fazla işletim sistemini aynı fiziksel bilgisayarda çalıştırmak, farklı işletim sistemlerini test etmek ve geliştirmek ve farklı yazılımları çalıştırmak için kullanılabilir.

***>> Aptitude ve apt Arasındaki Farklar Neledir ?***

- Linux dağıtımlarında kullanılan paket yöneticileridir.
- **Aptitude, apt'den daha kullanıcı dostudur.** Aptitude, kullanıcılara daha fazla seçenek sunar ve daha sezgisel bir arayüze sahiptir.
- **Aptitude, apt'den daha güçlüdür.** Aptitude, daha karmaşık paket işlemleri gerçekleştirebilir ve daha fazla bilgi sağlar.
- **Aptitude, apt'den daha yavaştır.** Aptitude, apt'den daha fazla işlem gerçekleştirdiği için daha yavaştır.
- 

***>> APPArmor Nedir ?***

- APPArmor, Linux dağıtımlarında kullanılan bir güvenlik aracıdır.
- APPArmor, uygulamaların sistemdeki kaynakları nasıl kullanabileceğini kısıtlamak için kullanılır. Bu, kötü amaçlı uygulamaların sisteme zarar vermesini önlemeye yardımcı olur.
- APPArmor, bir kural tabanlı güvenlik aracıdır. APPArmor, uygulamalara izin verilecek ve yasaklanacak kaynakları tanımlayan kurallar kümesi kullanır. Kural kümesi, bir .conf dosyasında depolanır.
- APPArmor, uygulamaların sistemdeki kaynakları nasıl kullandığını izlemek için bir çekirdek modülü kullanır. Uygulama bir kaynak kullanmaya çalıştığında, çekirdek modülü, uygulamanın izin verilip verilmediğini kontrol eder. İzin verilmezse, uygulamanın isteği reddedilir.
- APPArmor, Linux dağıtımlarında kullanılan güçlü bir güvenlik aracıdır. APPArmor, kötü amaçlı uygulamaların sisteme zarar vermesini önlemeye yardımcı olur.

*****************************************>> Makineye Bağlanma*****************************************

- ssh kgucluer@localhost -p 4242 Yazarak terminalden bağlan.

************>> UFW Hizmetinin Başladığını Kontrol Etmek************

- `sudo ufw status`

**>> SSH Hizmetinin Başladığını Kontrol Etmek**

- `sudo service ssh status`

******************************>> İşletim Sistemini Kontrol Etmek******************************

- `uname -a`

***>> User İşlemleri***

- Kullanıcı gruplarını kontrol etme
    
    `sudo groups <kullanıcı adı>`
    
- Yeni kullanıcı ekleme
    
    `sudo adduser <yeni kullanıcı adı>`
    
- Kullanıcıları listeleme
    
    `less /etc/passwd`
    
- Şifreleme politikaları düzenleme
    
    `sudo vim /etc/pam.d/common-password`
    
- Grup oluşturma
    
    `sudo groupadd <grup adı>`
    
- Gruba kullanıcı ekleme
    
    `sudo adduser <kullanıcı adı> <grup adı>`
    

***>> Hostname and partitions***

- Makine adı kontrol
    
    `hostnamectl`
    
- Makine adı değiştirme
    
    ```bash
    hostnamectl set-hostname <yeni makine adı>
    ```
    
- Makine yeniden başlat
    
    `sudo reboot`
    
- Bölümleri listeleme
    
    `lsblk`
    

*******************************>> LVM Nedir ?*** 

- LVM, bir Linux sistemindeki depolama alanını yönetmek için kullanılan bir araçtır. LVM, fiziksel diskleri veya disk bölümlerini gruplar halinde birleştirerek ve bu gruplardan mantıksal birimler oluşturarak çalışır.

***************>> SUDO***************

- Sudo kontrol
    
    `sudo --version`
    
- Yeni kullanıcıyı sudo grubuna ekleme
    
    `sudo adduser <yeni kullanici adi> sudo`
    
- /var/log/sudo klasöründeki dosya kontrolü
    
    `cd /var/log/sudo`
    

*************>> UFW*************

- UFW kontrol
    
    `sudo ufw status numbered`
    
- Yeni bağlantı noktası ekleme
    
    `sudo ufw allow <port numarası>`
    
- Bağlantı noktasını silme
    
    ```
    sudo ufw status numbered
    sudo ufw delete <silmek istediğin port numarası>
    ```
    

***************>> SSH***************

- SSH Nedir ?
    
    *SSH, iki bilgisayar arasında güvenli bir bağlantı oluşturmak için kullanılan bir ağ protokolüdür. SSH, kullanıcıların bir bilgisayardan diğerine dosya aktarmasını, komutlar çalıştırmasını ve uzak bir bilgisayarı yönetmesini sağlar.*
    
- SSH kontrol
    
    `sudo service ssh status`
    
- Yeni oluşturulan kullanıcı ile ssh kullanma
    
    `<yeni kullanıcı adı>@localhost -p 4242`
    

************>> Script Monitoring************

- [Monitoring.sh](http://monitoring.sh/) dosyasını açmak için
    
    `sudo vim /usr/local/bin/monitoring.sh`
    
- Crontab ayarlarını görüntülemek için
    
    `sudo crontab -u root -e`
