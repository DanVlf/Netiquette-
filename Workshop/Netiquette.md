# <u>**Netiquette**</u>

## Úvod

1.1 

- Jak se chovat v kyberprostoru                                                                                                                                             
  - Jak předejít napadení zařízení 

2.1

- Analyzace stáhnutých souborů (ověřování zdrojů, ...)
  - Jak pracovat s malware
   - Ukázky z reálných zkušeností s útoky 

3.1 

- WEB
  - Jak může vypadat reálný webový útok
  - Google Dorks

4.1

- Co je Social Engineering 
   - Kevin David Mitnick
   - Reálné případy 

5.1

- 5.1 Osobní doporučení







## 1.1 Jak se chovat v kyberprostoru 

​	**1.2 Jak předejít napadení zařízení** 

​			Možností, jak se bránit proti napadení našeho zařízení je několik. My se teď podíváme na ty nejzákladnější příklady, které by měl každý znát. 

​		**1.2.1 Detekce pochybného odkazu**

​			**1.2.1.1 Jak poznat podezřelý odkaz** 

​					Před tím, než klikneme na nějaký odkaz, měli bychom si zkontrolovat, kam nás zavede. Vždy je dobré zkontrolovat cestu, tu můžeme vidět buď ve vyhledávácím řádku, či v levém spodním rohu našeho vyhledavače. Odkazová cesta v levém spodním rohu se zobrazuje vždy, když najedeme kurzorem na nějaký odkaz, či jiné redirect tlačítko. V emailech se můžeme setkat s formou: klikněte <u>zde</u> . Právě v takových případech bychom si měli zkontrolovat levý spodní roh, kam nás odkaz odnese. Největší nevýhodou jsou v tomto případě mobilní zařízení, jelikož ty nemají primárně zabudovanou možnost prohlednutí odkazu, než na něj klikneme, proto není dobré klikat na tyto redirect tlačítka na mobilních zařízení  

​			**1.2.1.2 Příklady**

​						![legit1](C:\Users\Dan Volf\Desktop\Škola\SŠ\Workshop\Pics\legit1.jpg)

​	                    ![vicsusnelegit2](C:\Users\Dan Volf\Desktop\Škola\SŠ\Workshop\Pics\vicsusnelegit2.jpg)



![Evqi6NcXIAIx8Jm](C:\Users\Dan Volf\Desktop\Škola\SŠ\Workshop\Pics\Evqi6NcXIAIx8Jm.jpg)

![157799875_10223994489906668_7064688251012999723_o_1](C:\Users\Dan Volf\Desktop\Škola\SŠ\Workshop\Pics\157799875_10223994489906668_7064688251012999723_o_1.jpg)



**1.2.2  Analýza staženého obsahu** 

​				

​		**1.2.3 Typ Malware** 

​						  Malware je škodlivý kód, který se různými způsoby snaží poškodit zařízení oběti. Typů malware je mnoho, zde si ukážeme jen několik typů. 

|   Malware   |                          Vlastnost                           |
| :---------: | :----------------------------------------------------------: |
|    Virus    | Virus k šíření potřebuje již dopředu vytvořený funkční program. Viry jsou často připojeny k .exe či jiným typům souborů. |
| Trojský kůň | Trojský kůň je škodlivý program, který se vydává za neškodný. Uživatelé ho mohou lehce stáhnout do svého zařízení. |
|    Červ     | Červ se šíří díky zranitelnostem v softwarech. Jakmile se červ dostane do paměti, začne se rozšiřovat po celém zařízení. V některých případech se může dostat i do připojené sítě |
| Ransomware  | Ransomeware potlačí/zamítne přístup do vašich souborů, následně začne požadovat výkupné (většinou v cryptoměně) pro odemčení vašich dat |
|   Spyware   | Spyware tajně odposlouchává vaši on-line aktivitu, shromažďuje data sbírá osobní informace (uživatelská jména, hesla, ...) |

​		

​		**1.2.4 Zabezpečení heslem**

​				Dobré heslo je základ bezpečnosti pro vaše účty. Je důležité si uvědomit, že každý registrovaný učet spojený s naší osobou může obsahovat citlivá 				data. Pokud budeme mít takový profil špatně zabezpečen, může dojít k úniku takových dat a to vede k různě závažným důsledkům. Pokud si nejsme 				jisti při vytváření dobrého hesla, můžeme využít password generator který nám silné heslo vytvoří, dokonce může být upraveno podle vámi zadaných 				parametrů (délka, obsah znaků, ...)

​                                      	                                                                                                                                                                                                                                                                                                   

​                                                       ![image-20210302163944853](C:\Users\Dan Volf\AppData\Roaming\Typora\typora-user-images\image-20210302163944853.png)    





## 2.1  Analýza stáhnutých dat v našem zařízení 

​			Nástroje/služby, které použijeme: VirusTotal, Any.run  

​	**2.2 Jak pracovat s malware**

​		Zkontrolovat hash

```
70b6af3e51581d58adae074c52bcdd92
```

​		Nahrání souboru na VirusTotal 

​			![image-20210302131155439](C:\Users\Dan Volf\AppData\Roaming\Typora\typora-user-images\image-20210302131155439.png)

​	    Spuštění podezřelého souboru v Any.run. 

​		Malware jde analyzovat i manuálně. Jedena z nejednodušších cest jak získat nějaké informace o tom co malware dělá je ze stringů

​	

​	   -	Strings jsou česky textové řetězce, jsou to části textu obsažené v programu				![strings_vjyxkq](C:\Users\Dan Volf\Desktop\Škola\SŠ\Workshop\Pics\strings_vjyxkq.png)







​	**2.3 Ukázky z reálných zkušeností s útoky** 

​			**2.3.1 WannaCry**

​					Ransomeware. Původ nejspíše Severní Korea (KLDR).			                              																									  

​				   Dosud nakazil více než 250 000 počítačů ve více než 150 zemích světa.

​				   Útočník není zatím znám. Je potvrzeno, že útočník za 5 dní vydělal na malwaru přes 73000$.

​				   Zastavit se ho povedlo tak, že jeden z textových řetězců, který program obsahoval byla nezaregistrovaná doména. Tato doména fungovala jako 				   takový vypínač. Pokud by ji někdo zaregistroval ransomware by se nespustil a nezašifroval by soubory na nakaženém počítači.



​			**2.3.2 Ransomware v českých nemocnicích**

​						Českou nemocnici v Benešově napadl virus, který vyřadil z provozu všechny počítače. Provoz nemocnice byl zcela ochromen. Problémy začaly v 						noci, kdy se malware postupně rozšířil asi na 300 počítačů. 

​						Data již mohou být zašifrovaná a dostat se k nim může být i nemožné. Některé viry totiž klíče neuchovávají a nedokáží zajistit odemknutí souborů 						ani po zaplacení výkupného.

​					   Zde je tak hlavní otázkou, zda nemocnice uchovávala zálohu dat na oddělených discích nepřipojených do sítě, kam se virus nedostal. V krajním 					   případě by mohlo dojít až ke ztrátě uložených dat.

​					  A napadením stálo špatné zabezpečení sítě, zastaralý či neaktualizovaný software nebo nevhodné chování některého ze zaměstnanců. Podobné					  nákazy se často šíří za pomoci příloh e-mailů.

​					  Obnova systémů stála přes 40 milionů korun.

​                                                                           ![img](https://blog.malwarebytes.com/wp-content/uploads/2019/01/ryuk-ransom-note.png)



​				 Šlo o malware **Ryuk** - Cílí na instituce a firmy, které pracují s citlivými daty. Typicky zašifruje data do té doby, než je zaplaceno výkupné v bitcoinu.



 <img src="C:\Users\Dan Volf\Desktop\Škola\SŠ\Workshop\Pics\EtxNwXZXUAE6tUX.jpg" alt="EtxNwXZXUAE6tUX" style="zoom: 200%;" />





## **3.1 WEB** 



​	**3.2 Jak může vypadat reálný webový útok** 

​		K této ukázce jsme použili LAB od https://portswigger.net/. Následné rozebrání jednotlivých kroků by vám mohlo pomoci k následné teoretické ukázce.

​			**3.2.1 CSRF**

​				Funguje tak, že libovolná webová aplikace může posílat požadavky, a tím vykonávat různé změny na úplně jinou webovou aplikaci. Představte si 				například, že kliknutím na ![image-20210304111544725](C:\Users\Dan Volf\AppData\Roaming\Typora\typora-user-images\image-20210304111544725.png) na falešné kopii stránky vám změní heslo na Instagram.

​				V našem případě útočník zjistil, že při resetování hesla není přítomna žádná ochrana a tak díky speciálně vyrobenému requestu dokázal "přinutit"  				ostatní uživatele aby poslali request, který ani poslat nechtěli.

​			**3.2.2 Kroky útoku** 

​					1. Zrovna máte v prohlížeči otevřenou sociální síť, kde jste přihlášeni.   

![1](C:\Users\Dan Volf\Desktop\Škola\SŠ\Workshop\Pics\1.jpg)

​		

​				2. V tuto chvíli vám přijde e-mail od vaší školy, s tím, že si máte změnit heslo na školní výukový portál. V e-mailu se nachází odkaz, na který kliknete. 

​									 ![2](C:\Users\Dan Volf\Desktop\Škola\SŠ\Workshop\Pics\2.jpg)

​				3. Po kliknutí se dostanete na odkaz školního portálu, kde se nachází tlačítko "obnovit heslo". Na tlačítko kliknete a... 

![3](C:\Users\Dan Volf\Desktop\Škola\SŠ\Workshop\Pics\3.jpg)

​				4. Po kliknutí se nic nestane, tedy alespoň na první pohled.. Pokus se po nějaké době vrátíte na Instagram, zjistíte, že vaše přihlašovací údaje jsou 					změněny. 

![4](C:\Users\Dan Volf\Desktop\Škola\SŠ\Workshop\Pics\4.jpg)



 **3.3 Google Dorks**

​		Technika, která využívá Vyhledávání Google a další aplikace Google k vyhledání bezpečnostních mezer v konfiguraci a počítačovém kódu, které webové 		stránky používají.

​	**3.2.1 Syntaxe** 

​			Syntaxe u této zranitelnosti není potřeba tolik rozebírat. To co je pro nás výhodné je, že existuji desítky veřejných stránek se seznamy syntaxí pro náš 			průzkum zranitelností. 

```
SYNTAXE
"inurl:."domain"/"dorks" "
KAMERY
inurl:top.htm inurl:currenttime
inurl:”lvappl.htm”
FTP SERVERY
intitle:"index of" inurl:ftp
intitle:"index of" inurl:http after:2018
```

​																								Syntaxe se píše přímo do search baru

![image-20210304120125908](C:\Users\Dan Volf\AppData\Roaming\Typora\typora-user-images\image-20210304120125908.png)



​		Zde je příklad jak může vypadat live security kamera se zranitelností 

![image-20210304121241608](C:\Users\Dan Volf\AppData\Roaming\Typora\typora-user-images\image-20210304121241608.png)



## **4.1 Sociální inženýrství **



Sociální inženýrství je druh útoku na organizaci nebo jednotlivce, soustřeďující se na slabiny lidského faktoru. V dnešní době, vyznačující se rychlostí,			       anonymitou a větším zaměření na technologie, představuje takovýto druh útoku vážnou hrozbu.

​	**4.2 Twitter kauza**

​		Na Twitteru se ke konci minulého roku začali objevovat tweety od veřejně známých osobností/služeb s tím, že chtějí svým fanouškům/komunitě darovat 		peníze. "Zdvojnásobujeme všechny BTC platby, pošlete nám 1000$ a my vám zašleme 2000$ zpátky".  Pod touto zprávou byl odkaz na BTC peněženku, 		čeho jsme si například mohli všimnout je, že u všech tweetů byla stejná BTC peněženka. 

![img](https://btcmanager.com/wp-content/uploads/2020/07/elon-hack.jpg)

![img](https://btcmanager.com/wp-content/uploads/2020/07/hack.jpg)

  **4.3 Další způsoby**

​			Phishing - je podvodná technika používaná na Internetu k získávání citlivých údajů (hesla, čísla kreditních karet apod.)

​			Baiting - Při tomto způsobu útoku útočník nechá infikované CD, flashdisk nebo jiné paměťové médium na místě, kde jej oběť s velkou pravděpodobností 					      nalezne, například v koupelně, ve výtahu, na parkovišti. Poté již nechá pracovat zvědavost, se kterou oběť dříve či později vloží toto médium do 						  svého počítače. Tím dojde k instalaci viru, za pomoci kterého získá útočník přístup k počítači nebo celé firemní počítačové síti.

​		   IVR neboli telefonní phishing -Tato technika využívá falešného hlasového automatu (IVR) s podobnou strukturou jako má originální bankovní automat 														   ("Pro změnu hesla stiskněte 1, pro spojení s bankovním poradcem stiskněte 2"). Oběť je většinou vyzvána emailem k 														   zavolání do banky za účelem ověření informace.

**4.4 Kevin Mitnick**

​				V současné době se Kevin Mitnick snaží šířit povědomí o nebezpečí v podobě počítačových crackerů a phreakingů. Vlastní společnost podnikající v 				oboru bezpečnostního poradenství, *Mitnick Security Consulting*.

​				Za nelegální průnik do počítačových sítích byl v 90. letech odsouzen za počítačovou kriminalitu a za držení padělaných identifikačních dokumentů. Ve 				vězení strávil 5 let, propuštěn byl 21. ledna 2000. Bylo mu zakázáno používat jakékoliv komunikační technologie vyjma pevných linek. Později se mu u 				soudu podařilo dosáhnout zrušení zákazu přístupu na internet.

​				Kniha: The Art of Invisibility

​				![The Art of Invisibility by Kevin Mitnick | Mitnick Security](https://www.mitnicksecurity.com/hs-fs/hubfs/Book%20Covers/buy-invisibility.png?width=448&name=buy-invisibility.png)

**5.1 Osobní doporučení**

