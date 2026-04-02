# **Modul 1: Izazovi upravljanja lozinkama i password manageri**

## **Izazovi upravljanja velikim brojem lozinki (5 min)**

**Izvori:**

- https://pages.nist.gov/800-63-3/sp800-63b.html

- https://www.wpshealth.com/blog/?p=choosing-and-protecting-passwords

- https://cheatsheetseries.owasp.org/cheatsheets/Credential_Stuffing_Prevention_Cheat_Sheet.html

### **Zašto danas postoji veliki broj korisničkih računa?**

U suvremenom digitalnom okruženju gotovo svaka usluga zahtijeva stvaranje korisničkog računa. To uključuje osnovne digitalne alate poput e-maila i komunikacijskih platformi, ali i širok spektar dodatnih usluga kao što su društvene mreže, online bankarstvo, web trgovine, sustavi za učenje te mnoge druge.

Razvoj digitalnih usluga i potreba za personalizacijom sadržaja doveli su do značajnog povećanja broja korisničkih računa po pojedincu. Svaka platforma koristi korisničke račune za pohranu podataka, prilagodbu sadržaja i identifikaciju korisnika. Kao rezultat toga, broj potrebnih prijava kontinuirano raste.

Svaki korisnički račun zahtijeva jedinstvenu kombinaciju korisničkog imena i lozinke. Istovremeno, sigurnosne preporuke nalažu korištenje dugih, kompleksnih i nasumičnih lozinki. U takvim uvjetima postaje izrazito teško, a u praksi gotovo nemoguće, pouzdano zapamtiti toliki broj različitih lozinki bez sustavne pomoći.

Zbog toga se javlja potreba za organiziranim pristupom upravljanju lozinkama, koji omogućuje visoku razinu sigurnosti uz zadržavanje jednostavnosti korištenja.

### **Definicija upravljanja lozinkama**

Upravljanje lozinkama (password management) predstavlja skup praksi, procesa i alata koji omogućuju sigurno stvaranje, pohranu, zaštitu i ažuriranje lozinki.

Obuhvaća:

* definiranje pravila za izradu snažnih lozinki
* osiguranje sigurnog načina pohrane
* redovito ažuriranje i izmjenu lozinki
* izbjegavanje ponovne uporabe istih lozinki na različitim servisima

Cilj upravljanja lozinkama je osigurati da svaki korisnički račun ima jedinstvenu i sigurnu lozinku, uz minimalno opterećenje korisnika u svakodnevnom radu. Time se postiže ravnoteža između sigurnosti i praktičnosti.

### **Loše prakse upravljanja lozinkama**

Zbog kompleksnosti upravljanja velikim brojem lozinki često se koriste nesigurne metode koje pojednostavljuju pristup, ali značajno povećavaju sigurnosne rizike.

Najčešće loše prakse uključuju:

* **Zapisivanje lozinki na fizičke medije (papir)**
  Takvi zapisi mogu biti izgubljeni ili dostupni neovlaštenim osobama.

* **Pohranjivanje lozinki u nezaštićene digitalne dokumente**
  Tekstualne datoteke bez enkripcije lako su dostupne zlonamjernim programima ili drugim korisnicima uređaja.

* **Korištenje jednostavnih i predvidljivih lozinki**
  Lozinke poput „123456“ ili „password“ lako se otkrivaju automatiziranim napadima.

* **Ponovna uporaba iste lozinke na više servisa**
  Ova praksa predstavlja jedan od najvećih sigurnosnih rizika.

Najveći problem ponovne uporabe lozinki je lančana kompromitacija. U slučaju da dođe do sigurnosnog incidenta na jednoj platformi i curenja korisničkih podataka, ista lozinka može se iskoristiti za pristup drugim servisima.

Napadači često koriste automatizirane metode poput *credential stuffing* napada, gdje se ukradene kombinacije e-maila i lozinki testiraju na velikom broju različitih sustava.

Posljedice takvih napada mogu uključivati:

* neovlašten pristup e-mail računima
* krađu identiteta
* kompromitaciju poslovnih ili privatnih podataka
* financijsku štetu

Jedna sigurnosna slabost na manje važnom servisu može tako dovesti do ozbiljnih posljedica na ključnim korisničkim računima.

## **Prednosti korištenja password managera (7 min)**

**Izvori:**

- https://ssd.eff.org/module/creating-strong-passwords

- https://bitwarden.com/help/bitwarden-security-white-paper/

- https://bitwarden.com/compliance/

### **Što je password manager i kako štiti podatke?**

Password manager je specijalizirana softverska aplikacija namijenjena sigurnom upravljanju lozinkama i drugim osjetljivim podacima.

Može se opisati kao digitalni sef u kojem su svi podaci zaštićeni enkripcijom. Enkripcija pretvara podatke u nečitljiv oblik koji je moguće dešifrirati isključivo uz odgovarajući ključ.

Pristup tom sefu omogućuje jedna glavna lozinka – **MASTER lozinka**.

Karakteristike MASTER lozinke:

* predstavlja jedini ključ za pristup svim podacima
* ne pohranjuje se u čitljivom obliku
* poznata je isključivo korisniku

Ovakav model omogućuje korištenje velikog broja kompleksnih lozinki bez potrebe za njihovim pamćenjem.

### **Prednosti korištenja password managera**

#### **1. Generiranje snažnih i jedinstvenih lozinki**

Password manager omogućuje automatsko generiranje lozinki koje zadovoljavaju visoke sigurnosne standarde. Takve lozinke su:

* nasumične
* duge
* kombiniraju različite vrste znakova

Time se eliminira potreba za ručnim osmišljavanjem lozinki i značajno smanjuje rizik od kompromitacije.

#### **2. Eliminacija ponovne uporabe lozinki**

Za svaki servis može se koristiti jedinstvena lozinka bez dodatnog opterećenja korisnika. Time se sprječava lančana kompromitacija u slučaju sigurnosnog incidenta.

#### **3. Automatsko popunjavanje prijavnih podataka (Autofill)**

Password manager prepoznaje web stranice i automatski nudi unos odgovarajućih podataka. Prednosti ove funkcionalnosti uključuju:

* ubrzavanje procesa prijave
* smanjenje pogrešaka pri unosu
* povećanje sigurnosti (izbjegavanje ručnog unosa na sumnjivim stranicama)

#### **4. Zaštita od phishing napada**

Password manager uspoređuje URL adresu web stranice s onom koja je pohranjena u bazi podataka.

Ako adresa nije identična:

* neće se ponuditi automatsko popunjavanje
* korisnik dobiva signal da stranica može biti lažna

Ova funkcionalnost predstavlja važan zaštitni mehanizam protiv sofisticiranih phishing napada.

### **Što password manager nije?**

Password manager nije zamjena za sve sigurnosne mjere.

NE:

* eliminira potrebu za autentifikacijom
* štiti od svih vrsta napada
* može spriječiti sigurnosne incidente uzrokovane nepažnjom korisnika

DA:

* koristiti snažnu MASTER lozinku
* primjenjivati dodatne sigurnosne metode (2FA)
* biti oprezan pri otvaranju sumnjivih sadržaja

### **Uvod u Bitwarden**

Bitwarden je password manager koji se ističe kombinacijom sigurnosti, transparentnosti i dostupnosti.

#### **Open-source pristup**

Bitwarden je open-source rješenje, što znači da je njegov izvorni kod javno dostupan. To omogućuje:

* neovisnu sigurnosnu analizu
* veću transparentnost rada sustava
* brže otkrivanje i ispravljanje potencijalnih ranjivosti

#### **Zero-Knowledge arhitektura**

Bitwarden koristi model u kojem:

* se svi podaci šifriraju lokalno na uređaju
* server nikada ne prima nešifrirane podatke
* pristup podacima nije moguć bez MASTER lozinke

To znači da:

* ni pružatelj usluge nema pristup korisničkim lozinkama
* kontrola nad podacima ostaje isključivo kod korisnika

#### **Kriptografska sigurnost**

Bitwarden koristi moderne kriptografske standarde, čime se osigurava visoka razina zaštite podataka.

#### **Funkcionalnosti relevantne za svakodnevnu upotrebu**

Bitwarden nudi niz funkcionalnosti koje olakšavaju upravljanje lozinkama:

* sinkronizaciju između uređaja,
* dodatke (ekstenzije) za web preglednike
* sigurno dijeljenje podataka unutar organizacija ili timova
* pohranu dodatnih osjetljivih informacija

#### **Prikladnost za edukaciju i praksu**

Zbog dostupne besplatne verzije i jednostavnog sučelja, Bitwarden je posebno prikladan za:

* početnike koji prvi put koriste password manager
* edukacijske programe
* napredne korisnike koji žele veću kontrolu nad sigurnošću

Istovremeno, napredne opcije omogućuju i profesionalnu primjenu u poslovnom okruženju.

Na temelju strukture vašeg dokumenta i kvizova koje ste pripremili, evo razrađenog sadržaja za **Modul 2**. Sadržaj je strukturiran tako da izravno priprema polaznike za pitanja o izradi računa, sučelju i generatoru lozinki.

-----

# **Modul 2: Bitwarden sučelje i generiranje lozinki**

## **1. Izrada korisničkog računa (8 min)**

**Izvori:**

  - [https://bitwarden.com/help/create-your-account/](https://www.google.com/search?q=https://bitwarden.com/help/create-your-account/)
  - [https://bitwarden.com/help/master-password/](https://bitwarden.com/help/master-password/)

### **Prvi koraci i sigurnosna pravila**

Izrada Bitwarden računa prvi je korak prema potpunoj kontroli nad vašom digitalnom sigurnošću. Proces započinje registracijom e-mail adrese, ali ključni element zaštite vaših podataka događa se u trenutku kreiranja **Master lozinke**.

Bitwarden ne zahtijeva unos suvišnih osobnih podataka poput broja telefona, jer se njegova sigurnost temelji na snažnoj enkripciji, a ne na prikupljanju podataka.

### **Važnost Master lozinke**

Postavljanje snažne Master lozinke najkritičniji je korak pri izradi računa. Budući da Bitwarden koristi **Zero-Knowledge** arhitekturu, vaša lozinka se nikada ne šalje na njihove servere u čitljivom obliku.

**Što se događa ako zaboravite Master lozinku?**

  * **Gubitak pristupa:** Ako zaboravite Master lozinku, a niste prethodno spremili ili zapisali svoj **sigurnosni ključ (Recovery Key)**, vaši podaci postaju trajno nedostupni.
  * **Nema resetiranja:** Za razliku od uobičajenih web stranica, Bitwarden podrška **ne može** resetirati vašu lozinku niti vam je poslati na e-mail jer je oni jednostavno ne znaju.

### **Password Hint (Podsjetnik)**

Prilikom izrade računa nudi vam se opcija "Password Hint". To nije zamjenska lozinka, već kratki podsjetnik koji vam može pomoći da se sami sjetite Master lozinke ako zapnete. On je javan u smislu da ga sustav može poslati na vaš e-mail, stoga nikada nemojte upisivati samu lozinku kao podsjetnik.

-----

## **2. Bitwarden sučelje (5.5 min)**

**Izvor:**

  - [https://bitwarden.com/help/vault-guide/](https://www.google.com/search?q=https://bitwarden.com/help/vault-guide/)

### **Upoznavanje s elementima sučelja**

Sučelje Bitwardena dizajnirano je da bude jednostavno i pregledno, omogućujući brz pristup svim alatima. Glavni dijelovi koje ćete svakodnevno koristiti su:

  * **My Vault (Moj trezor):** Središnje mjesto gdje se nalazi lista svih vaših spremljenih elemenata (lozinke, kartice, bilješke).
  * **Gumb "+" (Add Item):** Nalazi se u gornjem ili donjem kutu (ovisno o uređaju) i služi za ručno dodavanje novog zapisa u trezor.
  * **Generator:** Poseban tab ili alat namijenjen brzom stvaranju novih, kompleksnih lozinki.
  * **Settings (Postavke):** Ovdje upravljate tehničkim postavkama računa, mijenjate jezik sučelja ili omogućujete dodatne sigurnosne opcije poput dvorazinske autentifikacije (2FA).

-----

## **3. Generiranje lozinki pomoću Bitwardena (12 min)**

**Izvori:**

  - [https://bitwarden.com/help/generator/](https://bitwarden.com/help/generator/)
  - [https://bitwarden.com/password-generator/](https://bitwarden.com/password-generator/)

### **Kako funkcionira Bitwarden generator?**

Generator lozinki je alat koji eliminira potrebu da sami smišljate lozinke. On osigurava da svaka vaša lozinka bude otporna na napade pogađanjem (brute force) kombinirajući veliku duljinu i raznolikost znakova.

### **Vrste generiranih zapisa**

Unutar generatora možete birati između dva glavna formata:

1.  **Password (Lozinka):** Niz nasumičnih znakova (npr. `g7#K9!vL2p$m`). Ovo je najsigurnija opcija za većinu servisa.
2.  **Passphrase (Lozinka u obliku fraze):** Niz nasumičnih riječi (npr. `kruh-oblak-planina-sunce`). Lakše se pamti i prepisuje, a i dalje nudi visoku razinu sigurnosti zbog svoje duljine.

### **Napredne postavke generatora**

Kako biste prilagodili lozinku zahtjevima različitih web stranica, možete koristiti dodatne opcije:

  * **Duljina lozinke:** Preporučuje se minimalno 12-16 znakova.
  * **Avoid Ambiguous Characters (Izbjegni dvosmislene znakove):** Ova opcija isključuje znakove koji slično izgledaju (npr. broj `0` i slovo `O`, ili malo `l` i broj `1`), što olakšava ručno prepisivanje ako je potrebno.
  * **Generiranje korisničkih imena:** Bitwarden također može generirati nasumična korisnička imena ili e-mail aliase, što dodatno štiti vašu privatnost.

### **Analiza sigurnosti**

Smatrajte lozinku poput `g7#K9!vL2p$m` standardom sigurnosti. Jednostavne lozinke poput `Ljeto2024` ili `Korisnik123!` podložne su napadima rječnikom i lako se pogađaju, bez obzira na to što sadrže jedno veliko slovo ili uskličnik. Pravu snagu daje isključivo **nasumičnost** koju pruža generator.
