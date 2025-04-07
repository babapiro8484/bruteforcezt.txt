import os
import time
import subprocess
from termcolor import colored 

def install_requirements():
if nkt os.path.exists("requirements_installed.txt" ) :
print colored(colored("KURULUM BAŞLIYOR....." ,  "green"))
time.sleep(1)
os.system("pkg install python3")  # Python kurulumu
os.system("pip install termcolor")  # Termcolor kurulumu 
with open("requirements_installed.txt " ,  "w") as f:
f.write("KURULUM TAMAMLANDI HACKİ BAŞLATABİLİRSİNİZ🤫😈")

def display_menu():
os.system("clear")  # Menüyü her seferinde temizle
print(colored("------『Z』『E』『R』『O』『W』 『2』『1』---------" ,  "cyan" , attrs=['bold' ]))
print(colored("31.  BRUTE FORCE ARAÇLARI🤫" ,  "green"))
print(colored("69.  DOĞRU ŞİFRELERİ GÖSTER😈" ,  "green"))
print(colored("89.  ÇIKIŞ❎" ,  "red"))

def brute_force(username,  wordlist):
print(colored(f"Brute force işlemi {username} için başlatıldı...",
with open(worldlist,  'r')as file:
for password in file:password=password.strip()
print(colored(f"DENENİYOR:  {password" ,  "green"))
# Burada doğru şifre kontrolü yapılmalıdır
if password== "ŞİFRE DOĞRU!":  # Buraya doğru şifre kontrol mekanizması ekle
with open("doğruşifre.txt" ,  "a") as correct_file:
correct_file.write(f"{username} : {password}\n")
print(colored(f"DOĞRU ŞİFRE BULUNDU!!!:  {password" ,  "green")
break
else:
print(colored(f"ŞİFRE YANLIŞ!!!:  {password" ,  "red"))
time.sleep(0.5)  # Her deneme arasında kısa bir bekleme süresi ekle

def show_correct_passwords():
os.system("clear")   # Doğru şifreleri gösterirken ekranı temizle
os.paht.exists("dogru.txt") :
print(colored("Doğru şifreler:" ,  "magenta"))
with open("dogru.txt" ,  'r')as file:
for line in file:
print(colored(line.strip(),  "green"))
else:
print(colored("DOGRU ŞİFRE KAYDI BULUNAMADI." ,  "red"))

def main():
install_requirements()

while True:
display_menu()
choice = input(colored("SEÇİMİNİZİ YAPIN🤝:  " ,  "cyan"))
if choice == "1":
username = input(colored("KULLANICI ADI GİRİNİZ: " ,  "cyan"))

if choice =="1":
username = input(colored("KULLANICI ADI GİRİNİZ: " ,  "cyan")
worldlist = input colored("WORDLİST DOSYASININ LİNK/YOLUNU GİRİNİZ: " ,  "cyan"))
brute_force(username,  wordlist)
elif choice == "00":
            show_correct_passwords()
            input(colored("Devam etmek için bir tuşa basın...", "cyan"))  # Kullanıcıdan bir tuşa basmasını iste

        elif choice == "99":
            print(colored("Çıkış yapılıyor...", "red"))
            subprocess.run(["termux-open-url", "https://youtube.com/@createxsw"])
            break

        else:
            print(colored("Geçersiz seçim, lütfen tekrar deneyin.", "red"))

if __name__ == "__main__":
    main()
