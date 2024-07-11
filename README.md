# **Swappify.app**
O [aplicatie web](http://swappify.app "aplicatie web") simpla si intuitiva pentru schimbarea trasaturilor faciale(deepfake)!

## Descriere

V-ati dorit vreodata ca profesorul vostru de fizica sa fie chiar **Albert Einstein**? Sau poate ca **Marie Curie** sa va explice misterele chimiei? Acum totul este posibil fara a irosi resurse pe makeup profesional si actori, puteti face totul online, usor si rapid pe site-ul nostru.

### De ce?

Am realizat că o problemă principală a sistemului de învățământ românesc este lipsa creativității în predare. Copiii s-au schimbat, si odata cu acestia si nevoile lor au suferit modificari.Intr-o era a tehnologiei atentia si dedicarea nu mai pot fi singurele virtuti ale elevilor. Aceștia nu rețin eficient lectiile atunci când sunt predate monoton și plictisitor. Cum ar fi, de exemplu, ca teorema relativității să fie predată chiar de faimosul fizician **Einstein**? Ați spune că e **imposibil**, că acesta nu mai trăiește și chiar dacă am realiza acum un video cu o replică de-a lui, ar costa foarte mulți bani!
**Dar cum ar fi daca totul s-ar putea realiza cu o camera video si putina creativitate?**

### Cum functioneaza?
Cu ajutorul inteligentei artificiale, care a devenit o unealta indispensabila in secolului 21, putem modifica trasaturile faciale ale orcarei persoane cu orice fata doriti!
### De ce sa ne folositi?
Alte servicii au
- timp de asteptare mare (uneori chiar cate 12 ore!)
- calitate inferioara 

Noi folosim un model revolutionar care eficinetizeaza timpul de asteptare!
Fiecare secunda (o secunda=25fps) este procesata in **o secunda** (cu o placa mid range)!
Interfata este usor de utilizat, oferind o experienta minunata si celor mai putin experimentati.!
### Forumul
Pentru ca in viata totul e mai frumos cand imparti, am decis sa realizez si un forum in care fiecare utilizator isi poate incarca videoclipul procesat, plus un sistem de comentarii si upvotes(like/dislike), pentru a putea fi folosit de si mai multe persoane!
- Fiecare videoclip procesat are optiunea de a fi postat.
- Daca utilizatorul decide sa posteze videoclipul, acesta va fi redirectioant catre o pagina pentru a realiza postarea, punand un titlu si o descriere adecvata.
- Dupa validare, postarea devine publica!

## Descriere tehnica
swappify.app este un software format din 2 parti:
- **Aplicatia care realizeaza deepfakeul**
- **Site-ul propiu-zis, care reprezinta o interfata intuitiva a aplicatiei, care dispune si de un forum pentru impartasirea creatiilor realizate**
### Masuri de securitate luate
Deoarece stiu ca acest proiect poate fi folosit in scopuri negative, am decis sa iau cateva masuri de securitate:
- verificarea automata pentru continut **NSFW** prin utilizarea librariei [OpenNSFW2](https://github.com/bhky/opennsfw2 "OpenNSFW2")
- (optional) verificarea manuala, in panoul de administrator
### Limbaje de programare utilizare si librarii
- Frondendul a fost realizat in **HTML,CSS si JS**, utlilzand **Bootstrap** ca framework
- Backendul a fost realizat in **PHP, MYSQL**(pentru baza de date)
- Aplicatia propriu-zisa a fost realizata in **Python**
#### Librarii
- pentru aplicatia de deepfake si conexiunea cu baza de date am utilizat **insightface**,**OpenCV**,**tensorflow**,**onnxruntime**,**numpy**,**mysql** ,**OpenNSFW2**

## Cerinte sistem
### Pentru utilizator
Orice browser modern
### Pentru server
Serverul pe care l-am folosit pentru lansarea beta a fost compus din:
- Procesor (CPU) **I7-12700KF** 12 cores 20 threads
- **32 GB RAM**
- Placa video (GPU-cel mai important component pentru acest proiect) **RTX 4070 12GB**
- **500 gb HDD** pentru stocarea de continut video si a imaginilor
- **128gb SSD** pentru sistemul de operare si a aplicatiilor necesare

## Alte informatii
- Cea mai importanta componenta a acestei aplicatii a fost placa video, deoarece, ca  pentru toate aplicatiile care folosesc machine learning, acesata foloseste resursele placii video.
- Ca fapt divers, aceasta placa video reuseste sa procesese undeva intre 20-25 de cadre pe secunda(fps), depasind si 60 in unele cazuri cand videoclipul trimis de utilizator e de o calitate inferioara.
