A sample command-line application with an entrypoint in `bin/`, library code
in `lib/`, and example unit test in `test/`.

# Belajar Import Library Dart

- setelah buat library push ke github
- lalu muncul banyak error dll ketika pub get nya

## Terus saya pakai:

dart pub outdated

dart pub upgrade --dry-run

atau 

dart pub upgrade

dan cek pubspec.yaml

habis itu lakukan ini lagi :

dart pub get

- Result : 
Resolving dependencies... (2.5s)
Got dependencies!

- Pakai Packages dari luar:
import 'package:belajar_dart_library/hello.dart' as belajar; 

untuk menghindari nama function atau nama package dll yang konflik atau duplikat.
contoh nya di folder bin/coba_import.dart

as belajar itu jadi prefix nya.

## Referensi pas Push ke github :
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#adding-your-ssh-key-to-the-ssh-agent

Generate key pair, github prefers the "Ed25519 algorithm"

ssh-keygen -t ed25519 -C "your_email@example.com"
It still allows using rsa for systems that don't support Ed25519

ssh-keygen -t rsa -b 4096 -C “youremail@example.com”

## Contoh Compile file exe windows di dart

dart compile exe bin/namafile.dart -o nama-app

habis itu nanti jadi file nya apptestnya (Windows)

bisa di running di terminal dgn cara :
./hasilcompile

Karena saya pilih nama nya 'apptestnya'
maka saya tinggal ketik ./apptestnya

nanti muncul output hasil file yg di compile nya.