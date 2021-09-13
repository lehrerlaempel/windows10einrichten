# Tutorial: Wie man Windows 10 sicher einrichtet (Eine Anleitung)
v 6.0 | Stand: September 2021 | Lizenz: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.de)

Weitere Anleitungen von uns findet man [hier](https://lehrerlaempel.github.io/anleitungen/)!

# Vorwort
Diese Anleitung soll dabei helfen, Windows 10 sicher einzurichten. Mit *sicher* ist dabei einerseits ein so datenschutzfreundliches und schwer anzugreifendes Windows wie möglich gemeint. Andererseits soll sich diese Anleitung auf Maßnahmen beschränken, die durchschnittliche Anwender:innen nicht überfordern und die alltägliche Benutzung des Systems möglichst wenig beeinflussen. Es geht hier also explizit nicht um ein möglichst gehärtetes System, sondern um so viel Sicherheit, wie ohne größere Einschränkungen "mit ein paar Mausklicks" eben möglich ist.

*Für sicherheitsempfindliche Einsatzszenarien sollte ernsthaft über einen vollständigen Verzicht auf Windows nachgedacht und stattdessen ein Linux-Betriebssystem erwogen werden. Zudem sollte in sensiblen Bereichen seriöse Hardware verwendet werden, die z.B. wie die Geräte von [Tuxedo](https://www.tuxedocomputers.com/) gut mit Linux zurechtkommt und auf freie Software setzen oder wie die [NitroPC und die NitroPads](https://shop.nitrokey.com/de_DE/shop) speziell gehärtet wurde. Für diese Anleitung gehen wir aber davon aus, dass Sie ein konventionelles Windows-Laptop verwenden, wie es sie in diversen Elektrofachmärkten zu kaufen gibt.*

Es wird übrigens dringend empfohlen, die Anleitung in der hier beschriebenen Reihenfolge zu durchlaufen. Sofern Sie aber bereits vor einem installierten System sitzen und nicht alles neu aufsetzen können oder wollen, können Sie sich aber auch selbstverständlich einzelne Kapitel herauspicken. Lieber nur einzelne Maßnahmen dieser Anleitung umsetzen, als keine!

Ihre Daten sollten Sie übrigens erst auf das Gerät kopieren bzw. mit dem Computer erst arbeiten, wenn Sie diese Anleitung vollständig durchlaufen habe, um die Sicherheit Ihrer Daten nicht zu gefährden.

Ein letztes Wort, bevor es endlich losgeht: Diese Anleitung beinhaltet lediglich allgemeine Empfehlungen. Es kann durchaus sein, dass diese Anleitung Fehler enthält oder aufgrund anderer Soft-/Hardware einige Punkte auf Ihrem System anders heißen. Haben Sie Mut, Ihr System selbst einzurichten. Wir möchten Sie mit dieser Anleitung dabei unterstützen. Aber zögern Sie bei Fragen bitte nie, sich im Internet oder bei fachkundigen Personen aus Ihrem Umfeld Hilfe zu holen.

# 1 Der erster Start
*(Diese Anleitung geht davon aus, dass Sie vor einem Windows10-System im Auslieferungszustand sitzen. Sollte dies nicht der Fall sein, können Sie einen bereits verwendeten Computer wie folgt wieder zurücksetzen: Start, Einstellungen, Update und Sicherheit, Wiederherstellung, Diesen PC zurücksetzen.)*

- Gerät einschalten.
- Sprache auswählen.
- Region auswählen.
- Tastaturlayout auswählen (sofern benötigt, kann im nächsten Schritt noch ein weiteres Layout gewählt werden, andernfalls einfach auf *überspringen* klicken).
- Weiter mit *Ich habe kein Internet*, weil wir Geräte wenn möglich immer offline Einrichten.
- Weiter mit *eingeschränktem Setup* (lokales Konto). 
- Den Windows 10-Lizenzvertrag annehmen. Was bleibt uns auch anderes übrig...
- Benutzername vergeben.
- Kennwort für den gerade erstellten User (Administrator) eingeben (min. 14 Zeichen) und merken, da ohne die Eingabe des Kennwortes Windows nicht mehr gestartet wird.
- 3 Sicherheitsfragen auswählen, beantworten und die Antworten merken/notieren.

Jetzt bietet Ihnen Microsoft noch diverse Features an. Generell gilt: Alle notwendigen Bestandteile des Betriebssystems sind bereits installiert. Bei allem was kommt, will Ihnen der Hersteller im Endeffekt primär die Zustimmung zu diversen Datenerhebungen abringen. Wir wählen also einfach immer die nicht vorausgewählte Option und willigen in möglichst wenig ein:

- Die Online-Spracherkennung nicht verwenden.
- Microsoft den eigenen Standort nicht verwenden lassen.
- *Mein Gerät suchen* ebenfalls abwählen.
- Nur erforderliche Diagnosedaten an Microsoft senden.
- Freihand und Eingabe nicht verbessern.
- Mithilfe von Diagnosedaten angepasste Erfahrungen abwählen.
- Apps Werbe-ID nicht verwenden lassen.
- Geräteübergreifenden Aktivitätsverlauf nicht nutzen.
- Hilfe von Cortana nicht annehmen.
- Ggf. eingeblendete Angebote des Herstellers bzgl. Garantie etc. überspringen bzw. einfach leer lassen. 
- Auch mögliche Angebote von Windows, das Gerät für bestimme Nutzungen zu personalisieren, mit einem Android Gerät zu verbinden, MS-Office zu nutzen oder z.B. OneDrive einzurichten, bitte alle ablehnen, überspringen bzw. *später einrichten* wählen

Nun startet Windows und der Desktop wird eingeblendet.

# 2 Updates
Als allererstes stellen wir sicher, dass unser System auf dem neusten Stand ist.

- PC mit dem Internet verbinden
- Windows 10 aktualisieren (Rechtsklick auf das Windows-Symbol, Einstellungen, Update und Sicherheit, Nach Updates suchen. Auch optionale Updates anzeigen lassen und installieren.)

# 3 BIOS
Wenn Sie in diesem Kapitel Fehler machen, kann das schnell dazu führen, dass Ihr Computer nicht mehr starten kann. Sollten Sie also unsicher sein, recherchieren Sie Ihre geplanten Schritte gründlich oder holen Sie sich fachkundigen Rat, **bevor** Sie anfangen, das BIOS zu verändern.

## 3.1 Konfiguration
Bevor wir uns näher mit dem Gerät beschäftigen, sollten wir zunächst die Einstellungen des BIOS überprüfen und bei Bedarf anpassen.

(*Das BIOS macht quasi den PC nach dem Start funktionsfähig und leitet im Anschluss das Starten eines Betriebssystems ein. Sollten Sie sich unter einem BIOS nichts vorstellen können, informieren Sie sich bitte unbedingt, wie ein Computer ganz grundlegend funktioniert. Ein guter Einstieg ist z.B. [dieses Video](https://www.youtube.com/watch?v=5PJZz04JGjs) der Sendung mit der Maus.*)

Starten Sie Ihren Rechner neu, unterbinden Sie den Start Ihres Betriebssystems und wechseln Sie in die Einstellungsoberfläche Ihres BIOS. Meist macht man das, indem man während des Starts F1, F2, F12, Enter oder ENTF mehrfach drückt. Das ist aber Herstellerabhängig und kann von Gerät zu Gerät variieren. Eine kurze OnlineRecherche nach *BIOS + Name des eigenen Gertätes* hilft meist schnell weiter.

Einmal im BIOS angekommen, empfehlen wir die folgenden Schritte:
- Lassen Sie im Boot-Menü nur die Festplatte mit Ihrem Betriebssystem als Startmedium zu und deaktivieren Sie das booten vom USB-Stick, sofern Sie das nicht benötigen
- Vergeben Sie für Ihr BIOS ein Administrator-Passwort, um unbefugte Änderungen zu verhindern.
- Aktivieren Sie die Unterstützung für Virtualisierungstechnologien.

## 3.2 BIOS-Update
Suchen Sie auf der Website Ihres Geräteherstellers nach einem ggf. vorhandenen Update für Ihr BIOS und installieren Sie dieses gemäß der Anleitung Ihres Herstellers.

# 4 Nicht benötigte Software entfernen
Starten Sie Ihren Computer neu. Lassen Sie uns nun vorinstallierte Software, die nicht benötigt wird, vom Gerät entfernen. Dies muss an drei unterschiedlichen Orten gemacht werden:

- Taskleiste/Start: Windows-Symbol drücken, dann öffnet sich das Startmenü. In diesem findet man im rechten Bereich diverse Icons und Verknüpfungen. Mit einem Rechtsklick können Sie die nicht benötigten nacheinander deinstallieren. Sollte diese Option im Einzelfall nicht verfügbar sein, wählen Sie "Vom Start lösen"
- Apps&Features: Windows-Symbol drücken und „Programme hinzufügen oder entfernen“ eintippen. Es öffnet sich das Menü Apps&Features. Hier werden installierte Programme angezeigt und können bei Bedarf deinstalliert werden.
- Programme&Features: Öffnen Sie das Menü Apps&Features (s.o.) im Vollbild. Oben rechts erscheint nun die Option "Programme und Features". Öffnen Sie dieses und deinstallieren Sie auch dort sämtliche nicht benötigte Software.

Generell gilt: So viel deinstallieren wir möglich! Eine Software, die nicht auf Ihrem System ist, kann Ihnen später auch nicht zum Verhängnis werden. Diese kann keine Daten sammeln, nicht angegriffen werden, etc. Sollten Sie sich bei einzelnen Programmen unsicher sein, klärt eine kurze Onlinerecherche meist schnell, was sich hinter nicht selbsterklärenden Programmnamen verbirgt.

*Wer Hilfe bei der Deinstallation von Apps möchte, kann sich z.B. das Tool [O&O App Buster](https://www.oo-software.com/de/ooappbuster) anschauen.*

# 5 Unerwünschte Funktionalitäten
Unser System ist auf dem neusten Stand, das BIOS ordentlich konfiguriert, überflüssige Software und Werbung entfernt. Bevor wir nun mit dem System arbeiten, sollten wir noch einige unerwünschte Funktionalitäten abschalten, die bei Windows 10 entgegen der Interessen der Nutzer:innen standardmäßig aktiviert sind.

## 5.1 Grundlagen
Erfahrene Nutzer:innen können hier "von Hand" z.B. anhand der Anleitungen des [BSI](https://www.bsi.bund.de/) viel erreichen, diese Anleitung richtet sich aber an Nutzer:innen ohne spezielle IT-Kenntnisse. Daher empfehlen wir an dieser Stelle, sich die Arbeit von einem Tool wie [O&O ShutUp10](https://www.oo-software.com/de/shutup10) abnehmen zu lassen. Hier bei Bedarf der Link zu einer [kurzen Anleitung](https://www.technikshavo.de/windows/windows-10-datenschutz-verbessern-mit-oo-shutup10-tutorial/).

Das schöne an *O&O ShutUp10* ist, dass ihnen jede einzelne Option ausführlich und für Laien verständlich erklärt wird! Klicken Sie dazu einfach auf den entsprechenden Eintrag. Das Tool blendet dann eine kurze verständliche Erklärung ein.

Alternativ kann auch eines der zahlreich weiteren vorhandenen Tools wie z.B. [W10Privacy](https://www.w10privacy.de/) für diesen Zweck verwendet werden. Bitte achten Sie jedoch darauf, für diese wichtige Aufgabe ein seriöses Programm aus vertrauenswürdiger Quelle zu verwenden!

## 5.2 W-LAN und Bluetooth
Ganz grundsätzlich sollten Sie auch Bluetooth und WLAN deaktivieren, sofern Sie diese nicht nutzen.

- Windows-Symbol drücken und nach *Bluetooth- und andere Geräteeinstellungen* suchen. Dort können Sie Bluetooth deaktivieren.
- Windows-Symbol drücken und nach *WLAN-Einstellungen* suchen. Dort können Sie zunächst das WLAN deaktivieren. Sofern Sie Ihr Gerät jedoch über WLAN mit dem Internet verbinden wollen, können Sie dort wenigstens das *verwenden zufälliger Hardwareadressen* aktivieren.

## 5.3 Windows-Netzwerkverhalten
Ihr Windows ist leider im lokalen Netz und teils sogar darüber hinaus sehr aktiv und bemüht darum, andere Computer zu finden. Um dem etwas Einhalt zu bieten, klicken Sie die Windowstaste und geben Sie dann "Netzwerkverbindungen" ein. In der sich daraufhin öffnenden Unterseite der Systemsteuerung wählen Sie auf der von Ihnen genutzten Netzwerkschnittstelle via rechter Maustatste *Eigenschaften*. Dort markieren Sie IPv4 und gehen dann auf *Eigenschaften*, danach auf *Erweitert*. Hier deaktivieren Sie nun im Reiter *WINS* sowohl den Eintrag *LMHOSTS-Abfrage aktivieren* und setzen dann einen Haken bei *NetBIOS über TCP/IP deaktivieren*.

# 6 Virenschutz
Windows 10 hat bereits einen von Haus aus integrierten Virenscanner. Die zahlreich vorhandenen Vergleichstests wie z.B. [dieser](https://www.av-test.org/de/antivirus/privat-windows/) legen nahe, dass dieser seine Arbeit nicht schlechter macht, als zusätzliche Anti-Viren-Software anderer Hersteller. Der große Vorteil: Ist der Windows-eigene Scanner einmal aktiviert, arbeitet dieser störungsfrei im Hintergrund und wird automatisch über die Windowsupdates aktuell gehalten. 

Drücken Sie auf das Windows-Logo, geben Sie "Viren- und Bedrohungsschutz" ein und stellen Sie in dem sich öffnenden Fenster sicher, dass dieser aktiviert ist.

Für alternative Anti-Viren-Software sollten Sie sich nur entscheiden, wenn Sie dafür einen guten Grund haben. Das Angebot der verfügbaren Software ist groß! Aber Vorsicht: Anti-Viren-Software hat auf Ihrem System sehr weitreichende Berechtigungen, Sie sollten dem Hersteller also unbedingt vertrauen.

# 7 Firewall
Es gibt von zahlreichen Herstellern Softwareprodukte zu kaufen, die Ihnen durch eine Software-Firewall mehr Schutz versprechen. Wer versteht, wie eine solche funktioniert und diese ordentlich konfigurieren kann, kann über den Einsatz einer solchen Nachdenken. Wird eine solche aber schlecht eingestellt, kann man sein effektives Schutzniveau aber auch durchaus senken und sich in falscher Sicherheit wiegen, statt wie erhofft sein System zu härten.

Durchschnittliche Nutzer:innen fahren also vermutlich am besten, wenn Sie zum Thema Firewall auf die Standardeinstellungen von Windows 10 vertrauen.

# 8 Festplatte verschlüsseln
Auch wenn man es nicht hofft: Ein Laptop kann im Zug vergessen werden, ein Computer bei einem Einbruch geklaut werden, oder aber es macht sich jemand in Ihrer Abwesenheit in böser Absicht an Ihrem Gerät zu schaffen, um Ihre Daten zu stehlen, manipulieren oder zu löschen. Wer sagt Ihnen denn, dass die nette Dame in Uniform am Flughafen, die Ihr Laptop kurz für einen angeblichen Sprengstofftest um die Ecke trägt, in Wirklichkeit nicht Ihre Daten von der Festplatte kopiert oder Ihnen Schadsoftware installiert?

Ein wichtiger Schutz für solche Fälle ist eine sogenannte Festplatten- oder Geräteverschlüsselung. Dadurch wird sichergestellt, dass Ihre kompletten Daten nur verschlüsselt auf dem Gerät gespeichert werden. Dadurch kommen mögliche Angreifer:innen an diese erstmal nicht heran und können zum Beispiel auch nicht ohne Weiteres Ihr Betriebssystem manipulieren.

## 8.1 BitLocker
Sofern Sie Windwos 10 Pro nutzen, bietet Ihnen Microsoft mit BitLocker einen einfachen Weg an, Ihre Festplatten zu schützen bzw. zu verschlüsseln:

Klicken Sie auf das Windwos-Symbol und geben Sie "BitLocker verwalten" ein. In dem sich nun öffnenden Fenster können Sie die Laufwerksverschlüsselung mit wenigen Mausklicks **für alle Ihre Laufwerke** aktivieren. 

Sichern Sie sich den im Installationsprozess angezeigten Wiederherstellungsschlüssel unbedingt auf einem externem Speichermedium oder drucken Sie diesen aus. Alternativ können Sie diesen auch mit "Microsoft Print to PDF" auf dem Destkop speichern und von Hand abschreiben. Egal welchen Weg Sie wählen: Stellen Sie sicher, dass Sie diesen abrufen können, sollte Ihr PC wegen technischer Probleme ohne diesen nicht mehr starten können! Selbstverständlich sollten Sie darauf achten, dass die Wiederherstellungsschlüssel nie in der Nähe des Laptops sind, da eine Angreiferin mit diesen leichtes Spiel hätte, Ihre Platte zu öffnen.

(Sollten Ihre Versuche, BitLocker zu aktivieren, in der Fehlermeldung enden, dass Ihr Gerät über kein TPM verfügt, finden sie z.B. [hier](https://computerfachmagazin.de/tutorials/microsoft/bitlocker-ohne-tpm-nutzen-oder-booten-mit-pin-password_3169/) oder [hier](https://www.giga.de/downloads/windows-10/tipps/bitlocker-in-windows-10-und-7-mit-und-ohne-tpm-so-geht-s/) eine Anleitung, wie Sie auch ohne TPM BitLocker aktivieren können.)

## 8.2 VeraCrypt
Sollten Sie Windows 10 Home nutzen, steht Ihnen BitLocker leider nicht zur Verfügung. Vielleicht möchten Sie sich ja aber auch nicht auf Bitlocker verlassen, weil Sie die [jüngsten Berichte über angebliche Sicherheitslücken](https://www.pc-magazin.de/news/windows-10-bitlocker-sicherheitsluecke-update-creators-update-patch-3197165.html) in der Software verunsichern, auch wenn diese nach unserer Einschätzung erstmal [wenig Praxisrelevanz haben](https://winfuture.de/news,52041.html).

Aber keine Sorge: Dank [VeraCrypt](https://www.veracrypt.fr/en/Downloads.html) (dem Nachfolger von TrueCrypt) müssen Sie nicht auf den wichtigen Grundschutz Festplattenverschlüsselung verzichten.

Installieren Sie sich zunächst VeraCrypt und verschlüsseln Sie dann mit diesem alle Ihre Festplatten. Anleitungen dazu finden Sie im Netz zuhauf, z.B. [hier](https://it-learner.de/das-betriebssystemlaufwerk-c-mittels-der-bitlocker-alternative-veracrypt-verschluesseln/) oder [hier](https://www.howtogeek.com/howto/6169/use-truecrypt-to-secure-your-data/).

# 9 Lauschabwehr
## 9.1 Physischer Schutz
Verfügt Ihr Computer über eine eingebaute Webcam, sollte diese bei Nichtgebrauch immer mit einer Abdeckung oder einem blickdichten Aufkleber versehen werden.

## 9.2 Software
In dem bereits erwähnten Tool [O&O ShutUp10](https://www.oo-software.com/de/shutup10) gibt es die Möglichkeit, ganz bequem softwareseitig Mikrofon und Webcam zu deaktivieren. Geben Sie beide nur für die Zeiträume für die Nutzung frei, wenn Sie diese auch tatsächlich benötigen.

## 9.3 BIOS
Sollten Sie Ihr Mikrofon und die Kamera erstmal nicht benötigen, gehen Sie noch einen Schritt weiter und deaktivieren Sie beide im bereits erwähnten BIOS ihres Computers.

# 10 Adminrechte & Trennung von Arbeitsbereichen
Ein zentrales Sicherheitsproblem von Windows ist, dass es meist direkt aus dem Administratorkonto heraus verwendet wird. Im Falle einer Infektion mit Schadsoftware wird es dieser dadurch deutlich einfacher gemacht, ebenfalls Administratorenrechte auf dem System zu erlangen. 

Ein weiteres Problem ist, dass man gerne verschiedene Tätigkeiten auf dem System voneinander Trennen würde. Wenn Sie alles in einem Nutzerkonto erledigen, laufen Sie immer Gefahr, dass z.B. die von Ihnen verwendete Software oder eventuelle Schadsoftware einen Überblick über Ihre Tätigkeiten, Kommunikationskanäle etc. bekommt. 

Um beide Probleme anzugehen, müssen wir unsere Arbeitsbereiche z.B. nach verschiedenen Projekten oder z.B. nach dienstlich und privat trennen. Dazu bieten sich im Wesentlichen zwei Wege an:

1. Entweder sie erstellen auf Ihrem PC mehrere Nutzerkonten ohne Adminrechte und arbeiten von nun an ausschließlich von diesen aus.
2. Oder aber Sie richten sich virtuelle Maschinen ein und arbeiten in diesen.

Zusätzliches Nutzerkonten sind einfach in der Handhabung, Virtualisierung bietet dafür mehr Schutz und mehr Möglichkeiten. Egal für welchen Weg Sie sich entscheiden: Nach diesem Kapitel sollten Sie Ihren ursprünglich auf dem Computer angelegten Nutzer mit seinen Adminrechten nicht mehr nutzen, um im Internet zu surfen, zu arbeiten, oder was auch immer Sie auf Ihrem System vorhaben.

## 10.1 Einrichten eines Nutzer-Kontos
Um ein Nutzerkonto ohne Administratorenrechte anzulegen, gehen Sie bitte wie folgt vor: Nach einem Klick auf das Windows-Symbol *Weitere Benutzer hinzufügen* eingeben. In dem sich dann öffnenden Menü kann über *Diesem PC eine andere Person hinzufügen* ein weiteres Konto angelegt werden, das ein anderes Passwort als der Administrator haben sollte. 

Sie können zum Beispiel einen Nutzer für private Angelegenheiten und einen für Dienstliches erstellen.

Nach dem Anlegen der Konten sollte der Rechner neu gestartet und von nun an nur noch über diese Nutzerkonten verwendet werden. Keine Sorge: Sie können weiterhin Dinge tun, die Administratorenrechte benötigen, z.B. Software installieren. Windows 10 wird Sie in solchen Fällen nach Ihrem Administratorenkennwort fragen und Ihnen kurzzeitig Administratorenrechte einräumen.

Wichtig: Bevor Sie die neuen Konten verwenden, sollten Sie unbedingt die Kapitel zum Entfernen überflüssiger Software sowie zum Deaktivieren unerwünschter Funktionalität für jedes neue Nutzerkonto nochmals durchlaufen.

## 10.2 Virtuelle Maschinen nutzen
Alternativ können Sie auch einfach Ihre eigentliche Nutzung des Systems in mehrere virtuelle Maschinen auslagern. So können Sie z.B. dienstliches und privates sauber voneinander trennen. 

Sie können sich virtuelle Maschinen wie eigene kleine Computer vorstellen, aus denen Schadsoftware erstmal nicht ohne weiteres ausbrechen kann. 

Sie können sich also zum Beispiel mit Hilfe der Software [VirtualBox](https://www.virtualbox.org/) mehrere virtuelle Maschinen (VM) anlegen. In der einen erledigen Sie ihren privaten Papierkrieg, in der anderen ihre berufliche Arbeit. In einer dritten experimentieren Sie mit neuer Software, in einer vierten besuchen Sie unseriöse Webseiten, etc. Sollten Sie sich in einer VM Schadsoftware einfangen, kann diese nicht die Daten in Ihren anderen VMs erreichen.

Wichtig: Den besten Schutz durch Virtualisierung erreichen Sie, wenn Sie ihr Host-System (Das Windows, das wir gerade einrichten) nur noch als Plattform für verschiedene VMs nutzen und in diesem selbst nicht mehr arbeiten, surfen, etc.

Mehr dazu in unserer separaten Anleitung zu diesem Thema: [Wie man Virtuelle Maschinen einrichtet](https://lehrerlaempel.github.io/vmseinrichten/)

# 11 Software installieren
Nun ist an an der Zeit, die zum Verwenden des Laptops benötigte Software zu installieren. *(Wir bewegen uns ab jetzt also entweder in einem Windows-Konto ohne Adminrechte oder in einer Virtuellen Maschine!)* Wann immer möglich, sollte man dabei auf [Freie Software](https://fsfe.org/freesoftware/freesoftware.de.html) zurückgreifen.

Eigentlich wäre es wichtig, Software zu überprüfen, bevor Sie diese Installieren. Unter Linux oder in AppStores auf dem Smartphone wird Ihnen das abgenommen. Unter Windows hingegen haben Sie das Problem, dass es keinen automatisch integrierten Mechanismus gibt, der sicherstellt, dass die von Ihnen heruntergeladene *irgendeinesoftware.exe* auch tatsächlich nur das vom Hersteller gebaute Programm enthält. Wer sagt Ihnen denn, dass die Datei nicht von Angreifer:innen auf dem Server oder dem Weg durchs Netz zu Ihnen manipuliert wurde? Wer sagt Ihnen eigentlich, dass in der Datei *firefox.exe* tatsächlich nur ein Browser und kein Trojaner steckt?

Leider ist das unter Windows bisher nicht ganz einfach. Fürs erste möchten wir daher auf [diese](https://roastedonion.wordpress.com/how-to/check-signatures/signatur-prufen/) Anleitung verweisen.

...doch vielleicht gibt es Licht am Ende des Tunnels: Mit dem **Windows Package Manager (winget)** gibt es seit Anfang 2021 ein Kommandozeilenprogramm, mit dem auch in Windows zentral über das Terminal Software installiert und - fast noch wichtiger - vor der Installation überprüft und später zentral geupdatet werden kann. Auch kann man so die Installation von viel Software sehr bequem automatisieren.

Wer keine Lust auf Kommandozeile hat, ignoriert das einfach und installiert sich Software ganz klassich über den Download der Installer von den Webseiten der Hersteller. Man sollte sich dann halt ernsthaft überlegen, ob man nicht wenigstens die Hash-Werte der Downloads überprüfen sollte. 

Allen anderen sei Kapitel **13.4 Windows Package Manager "winget"** dieser Anleitung wärmstens empfohlen :-)

## 11.1 WebBrowser
Browser sind ein zweischneidiges Schwert. Einerseits meist das Tor zu Welt und wichtiges Arbeitsmittel, andererseits aber auch eines der Haupteinfalltore für Angriffe und Schadsoftware. Es lohnt sich also, sich kurz über Auswahl und Konfiguration der verwendeten Browser Gedanken zu machen.

Anbei finden Sie einen Vorschlag für die Nutzung des TorBrowsers und als Ergänzung einen Mozilla Firefox. 

Übrigens: Browser sind als DIE Schnittstelle zum Internet auch ein interessantes Werkzeug, um Sie online zu identifizieren. Dabei werden heute neben Cookies auch diverse andere Merkmale herangezogen. Testen Sie doch einfach mal nach der Einrichtung von TorBrowser und Firefox zum Beispiel [hier](https://schemeflood.com/) oder [hier](https://coveryourtracks.eff.org/), welcher von beiden besser abschneidet.

### 11.1.1 TorBrowser
Als primären Browser empfiehlt es sich, den [TorBrowser](https://www.torproject.org/de/download/) zu verwenden, um beim Surfen möglichst wenig Spuren zu hinterlassen. Mehr zum Browser findet man zum Beispiel [hier](https://support.torproject.org/de/) oder [hier](https://www.heise.de/tipps-tricks/Der-Tor-Browser-Unzensiert-im-Darknet-surfen-3853797.html).

Die Anonymisierung funktioniert umso besser, je weniger man seinen TorBrowser verändert hat. Wir empfehlen also, den Tor-Browser in der ausgelieferten Standartkonfiguration zu betreiben.

### 11.1.2 Firefox
Manchmal benötigt man jedoch einen direkten bzw. nicht anonymisierten Zugang zum Internet. Manche Seiten und Dienste lassen sich z.B. nicht oder nur eingeschränkt über den Tor Browser nutzen.

Als alternativen Browser für diesen Zweck empfiehlt sich [Firefox](https://www.mozilla.org/de/exp/firefox/new/). Nachdem Sie diesen installiert haben, sollten Sie vor der ersten Nutzung allerdings noch die Einstellungen anpassen, die Sie nach Programmstart durch einen Klick auf die drei Balken oben rechts im Browserfenster und einen Folgeklick auf Einstellungen vorfinden.

#### 11.1.2.1 Konfiguration
Es lohnt sich generell, in Ruhe die einzelnen Menüs durchzugehen und sich den Browser je nach Geschmack anzupassen. Aus Datenschutz- bzw. Sicherheitsgründen sollten Sie jedoch mindestens die folgenden Punkte anpassen:

Im Menü **Allgemein**:
- Ganz am Ende der Seite unter *Verbindungs-Einstellungen* auf *Einstellungen* klicken. Am Ende dieser Seite *DNS über HTTPS aktivieren* aktivieren, um sogenannte Man-in-the-Middle-Angriffe deutlich zu erschweren.


Im Menü **Startseite**:
- Sowohl *Startseite und neue Fenster* als auch *Neue Tabs* auf *Leere Seite* einstellen


Im Menü **Suche**:
- Ändern Sie die *Standardsuchmaschine* auf eine datenschutzfreundliche Alternative wie z.B. [DuckDuckGo](https://duckduckgo.com/) oder [Startpage](https://www.startpage.com/).

Im Menü **Datenschutz und Sicherheit**:
- Wählen Sie unter *Verbesserter Schutz vor Aktivitätenverfolgung* die Option *streng*.
- Lassen Sie immer eine *Do Not Track Information* senden.
- Aktivieren Sie die Option *Cookies und Website-Daten beim Beenden von Firefox löschen*.
- Deaktivieren Sie entweder die Option *Zugangsdaten und Passwörter speichern*, oder aber vergeben Sie ein *Hauptpasswort*, falls Sie diese Option nutzen möchten.
- Lassen Sie eine *Chronik nach benutzerdefinierten Einstellungen anlegen* und aktivieren Sie die Option *Die Chronik löschen, wenn Firefox geschlossen wird*.
- Deaktivieren Sie sämtliche *Datenerhebung durch Firefox*.
- Wählen Sie *Nur-HTTPS-Modus in allen Fenstern aktivieren*

Im Menü **Sync**:
- Sofern Sie darauf verzichen können, melden Sie sich bitte nicht mit einem Firefox Konto an bzw. erstellen Sie kein solches.

#### 11.1.2.2 Add-ons
Durch das Installieren von Add-ons können Sie Ihrem Browser weiteren Schutz hinzufügen und das Surfen bequemer gestalten. Aber Achtung: Die Add-ons haben Zugriff auf das, was Sie im Browser machen. Sie sollten also nur vertrauenswürdige Programme installieren.

Zur Installation von Add-ons klicken Sie bitte in Ihrem Firefox-Browser auf die drei Balken oben rechts und dann auf *Add-ons*. Hier können Sie nun Erweiterungen aussuchen und installieren. Derzeit würden wir mindestens folgendes empfehlen:

- [uBlock Origin](https://addons.mozilla.org/en-US/firefox/addon/ublock-origin/) blockt ressourcenschonend Werbung und Tracking.

Wer etwas Geduld für die Einrichtung und einen hohen Schutzbedarf hat, kann sich noch die folgenden zwei Add-ons anschauen:
- [NoScript](https://addons.mozilla.org/de/firefox/addon/noscript/) schützt Sie vor unerwünschten aktiven Inhalten wie JavaScript, Flash oder Java, die häufig für das Ausbringen von Schadsoftware genutzt werden.
- [UserAgent-Switcher](https://addons.mozilla.org/en-US/firefox/addon/user-agent-string-switcher/) verändert den User-Agent und verschleiert so, welches Betriebssystem und welchen Browser Sie verwenden

Das sollte für die meisten Nutzer:innen genug des Guten sein. Wer seinen Browser noch weiter härten möchte, findet [hier](https://www.torbox.ch/?page_id=112) im oberen Drittel der Seite sowohl Anregungen für weitere Add-ons als auch weiterführende Möglichkeiten, Firefox zu konfigurieren.

## 11.2 E-Mail-Client
Sofern E-Mails auf Ihrem Computer nicht über den Browser abgerufen werden sollen, empfiehlt sich die Installation von [Thunderbird](https://www.thunderbird.net/de/), um Mails automatisch abrufen und auch offline verarbeiten zu können. Mit der aktuellen Version von Thunderbird wird auch das sichere Verschlüsseln von E-Mails zum Kinderspiel, aber dazu mehr in unserer Anleitung [Wie man eine sichere E-Mailverschlüsselung einfach einrichtet](https://lehrerlaempel.github.io/emailverschluesselung/).

Wichtig: Sofern Sie die Passwörter für Ihre E-Mail-Konten in Thunderbird speichern möchten, vergeben Sie auch hier unbedingt zuvor in den Einstellungen ein Hauptpasswort bzw. **Masterpasswort**, um Ihre Zugangsdaten zu schützen!


## 11.3 Office-Umgebung
Es gibt zahlreiche Office-Programme. Teilweise können Sie für diese erstaunlich viel Geld bezahlen, andere hingegen sind freie Software und damit kostenlos. Egal für welches Produkt Sie sich am Ende entscheiden: Wählen Sie im Optimalfall eine Software, die nicht ständig versucht, Ihre Dokumente in die Cloud hochzuladen oder Sie zum Anlegen eines Nutzerkontos zu zwingen.

Wir können Ihnen zum Beispiel das freie [LibreOffice](https://de.libreoffice.org/) wärmstens empfehlen.

## 11.4 Multimedia
### 11.4.1 Videos
Für das Abspielen von Videos empfiehlt es sich, den [VLC Media Player](https://www.videolan.org/vlc/) zu nutzen. Dieser kommt mit nahezu allen Videoformaten zurecht, kann übrigens auch streamen und spielt bei Bedarf auch Musik ab.

Zum Konvertieren und Zuschneiden von Videos empfiehlt sich [Handbrake](https://handbrake.fr/).

Auch für das aufnehmen von Videos, Screencasts, etc. gibt es eine gute freie Software: [OBS Studio](https://obsproject.com/).

### 11.4.2 Bilder
Für das Sortieren und Betrachten der eigenen Bilder inklusive kleinerer Arbeiten (wie z.B. das Ändern der Größe) können die in Windows bereits vorinstallierten Tools *Fotos* und *Paint* verwendet werden. Wer auf der Suche nach einer Alternative ist, sollte sich [XnView](https://www.xnview.com/de/) anschauen.

Wer hingegen intensiver mit und an Bildern arbeiten, aber nicht auf kommerzielle Produkte zurückgreifen möchte, dem sei [GIMP](https://www.gimp.org/) wärmstens empfohlen. Die Software kann - nach einer gründlichen Einarbeitung des Nutzers - nahezu alles.

## 11.5 Passwortmanager
Sichere Passwörter sind ein Thema für sich. Letztlich kommen aber die meisten seriösen Betrachtungen zu dem Thema zum Ergebnis, dass unsere Passwörter möglichst lang, maximal komplex und zufallsgeneriert sein sollten. Zudem sollten wir diese immer mal wieder ändern und überall andere Passwörter verwenden.

WIE?!?

Ganz einfach: Nutzen Sie einen Passwortmanger, der in einer lokalen Datei ihre Passwörter gut verschlüsselt ablegt und auch neue Passwörter für Sie generieren kann. So müssen Sie sich nur noch ein Masterpasswort für die Datenbank merken.

Unsere Empfehlung: [KeepassXC](https://keepassxc.org/) ist ein freier Passwortmanager. Wer bisher keinen Passwortmanager nutzt, sollte dringend in Erwägung ziehen, damit anzufangen. Mehr Informationen zum Thema findet man z.B. [hier](https://www.heise.de/tipps-tricks/Passwortmanager-So-verwalten-Sie-Ihre-Passwoerter-3934582.html) oder [hier](https://www.avg.com/de/signal/why-you-need-a-password-manager).

## 11.6 Weitere Software-Empfehlungen
Anbei noch ein paar Programme, deren Installation ernsthaft in Erwägung gezogen werden sollte:
- [7Zip](https://www.7-zip.org/) ist ein kleines freies Packprogramm, dass mit allen gängigen Archivtypen zurecht kommt.
- [Veracrypt](https://www.veracrypt.fr/) (der Nachfolger von TrueCrypt) ist eine Software zur Datenverschlüsselung und beherrscht auch die vollständige Verschlüsselung von Festplatten und Wechseldatenträgern.


# 12 Backups
Sofern Sie auf Ihrem Laptop mit Daten arbeiten, deren Verlust für Sie ein Problem wäre, sollten Sie sich direkt bei der Einrichtung Ihres Laptops eine BackUp-Strategie überlegen bzw. von Anfang an nach dem gewohnten Muster weiterhin regelmäßig Sicherungen Ihrer Daten vornehmen.

Wer bisher keine sinnvolle Lösung für regelmäßige Backups hat, anbei drei Vorschläge.

Zuerst aber noch kurz zur Grundregel: Egal welchen der unteren Vorschläge Sie am Ende umsetzen oder ob Sie einen anderen ganz eigenen Weg gehen: Am Ende des Tages sollten Ihre BackUps die folgenden Kriterien erfüllen:

- Sie sollten mindestens **3** Versionen Ihrer Daten haben: Die "Originale" auf Ihrem Computer sowie mindestens 2 Sicherungen (falls z.B. beim Sichern ein Problem entsteht, bleibt immer noch eine unversehrte Version).
- Ihre BackUps sollten auf mindestens **2** verschiedenen Speichermedien liegen (z.B. falls eines davon verloren oder kaputt geht).
- Mindestens **1** Sicherung sollte räumlich getrennt von Ihrem Laptop und den anderen BackUps aufbewahrt werden (z.B. bei einer Kollegin oder einem Verwandten zuhause, falls es z.B. bei Ihnen zu einem Brand, einem Einbruch oder einer Hausdurchsuchung kommt).
- Sämtliche BackUps sollten **verschlüsselt** sein (um diese vor unbefugtem Zugriff zu schützen).

## 12.1 Archive auf USB-Sticks
Sofern die zu sichernden Daten nicht das Volumen handeslüblicher USB-Sticks überschreiten (derzeit ca. 128GB), ist eine einfache mögliche Lösung, sich einfach 2 USB-Sticks zu besorgen. Mit Hilfe des bereits erwähnten [7Zip](https://www.7-zip.org/) erstellen Sie dann einfach immer Freitags in geraden Wochen auf dem einen und in ungeraden Wochen auf dem anderen Stick ein **verschlüsseltes** Archiv mit allen Ihren Daten. Einer der Sticks liegt dann z.B. zuhause, einer im Büro. 

Sofern Sie eine externe Festplatte haben, funktioniert ein solches vollständiges BackUp natürlich auch mit größeren Datenmengen. Erfahrungsgemäß macht das dann aber niemand regelmäßig, da das dann schnell mehrere Stunden benötigt.

## 12.2 Duplicati
Vor allem für größere Datenmengen bietet es sich daher an, ein Tool zu verwenden, dass nicht jedes Mal eine komplett neue Sicherung erstellt, sondern lediglich die Änderungen speichert. Man spricht hier dann meist von sogenannten inkrementellen BackUps. Hierzu empfiehlt sich z.B. die freie Software [Dulicati](https://www.duplicati.com/).

Das Tool ist eine Software, die verschlüsselte, komprimierte, inkrementelle Datensicherungen erstellt und diese auf Netzwerklaufwerke, integrierte oder externe USB-Festplatten oder Onlinespeicher übertragen kann. 

Die erste Sicherung benötigt recht lange. Aber von da an können Sie auch große Datenmengen über mehrere Terabyte in wenigen Minuten sichern.

[Hier](https://digitalcourage.de/sites/default/files/2018-11/bp_handout_duplicati_v0.7.pdf) finden Sie eine kurze Anleitung zum Einrichten des Tools.

## 12.3 Ganze VMs sichern
Das Arbeiten in virtuellen Maschinen hat nicht nur massive sicherheitliche Vorteile, sondern kann auch das Erstellen von BackUps deutlich vereinfachen. 

Falls Sie - wie oben erwähnt - mit VirtualBox Ihre VMs verwalten und diese bei der Installation auch verschlüsselt haben (eine Option, die z-B. bei den meisten Linux-Distributionen im Installationsprozess angeboten wird), können Sie diese einfach exportieren. So haben Sie nicht nur ein BackUp Ihrer Daten, sondern direkt ihre komplette Arbeitsumgebung inklusive aller installierten Programme und Einstellungen jederzeit griffbereit, um diese bei Bedarf auf einem anderen Computer zu importieren.

Beenden Sie dazu zunächst alle VMs. Klicken Sie dann in VirtualBox unter *Datei* auf *Appliance exportieren*. Wählen Sie nun die gewünschte VMs (Mehrfachauswahl möglich!). Wählen Sie das *Open Virtualization Format 2.0* und den Ort, an dem die ova-Datei gespeichert werden soll, die alle Ihre VMs enthält. 

Wichtig: Nur wenn Sie die Festplatten der VMs verschlüsselt haben, erhalten Sie sichere BackUps, die vor ungewolltem Zugriff geschützt sind!

Die so erstelle ova-Datei kann nun auf jedem beliebigen PC per Doppelklick importiert werden, sobald VirtualBox installiert ist.

# 13 Sonstiges
Hier noch ein paar Kleinigkeiten, die nicht zwangsläufig notwendig sind, den Betrieb auf Dauer aber erheblich verbessern:

## 13.1 Energieeinstellungen
Drücken Sie die Windows-Taste, geben Sie *Einstellungen für Netzbetrieb und Energiesparen* ein und öffnen Sie diese. Passen Sie die Einstellungen dort nach Ihren Wünschen an.

Drücken Sie die dann nochmal Windows-Taste, geben Sie *Systemsteuerung* ein und öffnen Sie diese. Wählen Sie unter *Hardware und Sound* unter *Energieoptionen* die Option *Netzschaltverhalten ändern*. Aktivieren Sie durch einen Klick auf das Schutzschild oben alle Optionen und deaktivieren Sie dann die Option *Schnellstart aktivieren*.

## 13.2 Taskleiste
Klicken Sie mit der rechten Maustaste auf eine freie Stelle Ihrer Taskleiste und öffnen Sie die *Taskleisteneinstellungen*. Wählen Sie nun unter *Schaltflächen der Taskleiste gruppieren* die Option *Wenn die Taskleiste voll ist* und öffnen Sie dann den Link *Symbole für die Anzeige auf der Taskleiste auswählen*. Dort setzten Sie bitte den Haken für *Immer alle Symbole im Benachrichtigungsbereich anzeigen*.

Machen Sie noch einen Rechtsklick auf eine leere Stelle der Taskleiste und wählen Sie unter *Suchen* die Option *ausgeblendet*.

## 13.3 Wiederherstellungspunkte nutzen
Öffnen Sie die Taskleiste und geben Sie *Wiederherstellungspunkt erstellen* ein. In dem sich öffenenden Fenster können Sie unter *erstellen* einen Wiederherstellungspunkt erstellen. Geben Sie diesem einen griffigen Namen um später nachvollziehen zu können, vor oder nach welcher Systemänderung Sie diesen erstellt haben.

Machen Sie vor allgen größeren Systemänderungen solche Wiederherstellungspunkte. Über die Schaltfläche *Systemwiederherstellung* auf der selben Menüseite können Sie so später jederzeit Ihr System (nicht die Nutzer:innen-Daten, nur das Betriebssystem) auf einen früheren Zustand zurücksetzen. Das spart oft viel Reparaturarbeit, manchmal sogar eine Neuinstallation des Systems.

## 13.4 Windows Package Manager "winget"
Hier ein paar Worte zum [Windows Package Manager "winget"](https://docs.microsoft.com/de-de/windows/package-manager/winget/) von Microsoft. Zum Start einfach mit der rechten Maustaste auf das Windows-Logo und dann auf *Windows PowerShell (Administrator)* gehen. In dem sich nun folgenden Fenster kann man mit folgenden Befehlen spielen:

- **winget install --id=exakteProgrammID  -e** installiert eine Software. Eine gute Übersicht der verfügbaren Programme und deren genaue Bezeichnung findet man auf [Winstall.app](https://winstall.app/apps). Einfach in das Suchfeld den Namen der gewünschten Software eingeben. Nach einem Klick auf die Software kommt dann eine Übersichtsseite, auf der sich auch der Befehl für die Installation findet.
- **winget list** erzeugt eine Liste der installierten Software inkl. exakter Versionsbezeichnung. Sind neuere Versionen in winget verfügbar, wird dies dahinter angezeigt.
- **winget upgrade ID** kann ein einzelnes Programm geupdatet werden, zu dem eine neue Version vorliegt. Dazu einfach *ID* durch die in der Liste oben aufgeführte ID ersetzen, also z.B. *winget upgrade Mozilla.Thunderbird*.
- **winget upgrade --all** installiert alle verfügbaren Updates.

Die Seite **[Winstall.app](https://winstall.app/apps)** bietet übrigens auch eine weitere interessante Funktion: Durch das klicken auf das Plus-Symbol kann man Software quasi in einen Warenkorb legen. Hat man alles benötigte ausgewählt, klickt man unten auf *Generate script*. Die Seite erstellt dann einen Befehl, der alle ausgewählten Programme nacheinander installiert. Über *Copy to clipboard* kann dieser in die Zwischenablage kopiert und in die PowerShell eingefügt werden. Alternativ kann man auch eine bat-Datei herunterladen, die nach einem Doppelklick die ausgewählten Programme installiert. Das spart viel Zeit und Nerven, die man sonst benötigt hätte, von Hand diverse Programme erst zu verifizieren, um sich dann durch das Installationsmenü zu klicken. Der Seite muss man übrigens nicht blind vertrauen: Der Syntax der Datei ist nahezu selbsterklärend: Ein Klick auf die Datei vor dem Ausführen mit der rechten Maustaste, dann *Bearbeiten* auswählen und schon kann man kontrollieren, was da gleich ausgeführt werden soll.

Übrigens: Bei der Installtion erscheint dann immer auch die Zeile *Der Installer-Hash wurde erfolgreich überprüft*. Alleine dafür lohnt es sich, einen Blick auf winget zu werfen. Alternativ müsste man nämlich von jeder einzelnen heruntergeladenen Exe den Hashwert und die kryptographische Signatur eigenständig prüfen. Und mal Hand aufs Herz: Wer macht das schon...

Falls winget auf Ihrem System noch nicht installiert ist und die oben erwähnten Befehel nur rote **Fehlermeldungen** aussprucken: [Hier](https://github.com/microsoft/winget-cli/releases) findet man auf GitHub die neuste Version des Tools. Einfach von der neusten Version die Datei *Microsoft.DesktopAppInstaller_8wekyb3d8bbwe.msixbundle* (oder so ähnlich) herunterladen und installieren. Danach müsste das funktionieren.

- - - -

***Herzlichen Glückwunsch, Sie haben es geschafft!***

***Sofern Sie tatsächlich alle oben beschriebenen Schritte durchgeführt haben, profitieren Sie zukünftig von einem soliden Grundschutz gegen die digitalen Bedrohungen im 21. Jahrhundert und die Misslichkeiten des digitalen Alltags.***

***Ein gut konfiguriertes Gerät ist jedoch kein Allheilmittel! Sie sollten stets vorsichtig mit Ihrer IT umgehen und vor allem bei der Installation von Software, dem Einstecken von Wechselmedien und dem Download von Daten auf vertrauenswürdige Quellen achten!***

- - - -

# 14 Langfristige Routinen
Bitte beachten Sie, dass diese Grundkonfiguration für einen sicheren Betrieb nicht ausreicht, da Ihr System z.B. von Microsoft im Rahmen von Updates immer wieder verändert wird. Auch Sie selbst als Nutzer:in ändern meist im Laufe der Zeit z.B. durch Installationen immer wieder Ihr System.

Sie sollten also alle paar Monate die folgenden Schritte durchführen, um sicherzustellen, dass Ihr System nach wie vor ordentlich konfiguriert ist:
- Windows-Symbol drücken und nach *WLAN-Einstellungen* suchen. In dem sich öffnenden Fenster unter *Bekannte Netzwerke verwalten* alle Netzwerke löschen, die auf Orte/Lokalitäten hindeuten, mit denen Sie nicht in Verbindung gebracht werden möchten.
- Prüfen, ob es verfügbare aber noch nicht automatisch installierte Windows-Updates gibt.
- Mit einer aktuellen Version des verwendeten Tools zum entfernen unerwünschter Funktionalität prüfen, ob z.B. durch Updates unerwünschte Features wieder aktiviert wurden.
- Prüfen Sie die auf Ihrem System installierte Software regelmäßig auf Updates! Anders als z.B. meist unter Android oder Linux werden Ihre Programme von Windows 10 nicht automatisch aktualisiert! (Allerdings kann Ihnen der Terminalbefehl *winget list* immerhin eine gute Übersicht der installierten Programmversionen anbieten und *winget upgrade --all* wenigstens einen Teil davon aktualisieren.)

# 15 Das Kleingedruckte
## 15.1 Fehlerteufel
Diese Anleitung wurde von [lehrerlaempel](https://github.com/lehrerlaempel) nach bestem Wissen und Gewissen erstellt. Wir haben die feste Absicht, diese im Laufe der Zeit an Änderungen der erwähnten Software anzupassen und um weitere Aspekte zu ergänzen.

Ihnen sind Fehler aufgefallen? Sie haben Verbesserungs- oder Änderungswünsche? Dann nehmen Sie gerne [Kontakt](https://lehrerlaempel.github.io/anleitungen/) mit uns auf. Wir sind tatsächlich sehr an Ihrer Rückmeldung interessiert!

Wir übernehmen explizit keinerlei Haftung für die hier getroffenen Aussagen oder möglicherweise daraus entstandene Datenverluste oder Schäden am Gerät. Wir haben diese Texte nach bestem Wissen und Gewissen verfasst, sind aber wie alle Menschen fehlbar.

## 15.2 Lizenz
Dieser Text steht unter einer CC-Lizenz, ist also quasi schöpferisches Gemeingut.

Sie dürfen:
- **Teilen** das Material in jedwedem Format oder Medium vervielfältigen und weiterverbreiten
- **Bearbeiten** das Material remixen, verändern und darauf aufbauen

Der Lizenzgeber kann diese Freiheiten nicht widerrufen solange Sie sich an die Lizenzbedingungen halten.

Unter folgenden Bedingungen:
- **Namensnennung** Sie müssen angemessene Urheber- und Rechteangaben machen, einen Link zur Lizenz beifügen und angeben, ob Änderungen vorgenommen wurden. Diese Angaben dürfen in jeder angemessenen Art und Weise gemacht werden, allerdings nicht so, dass der Eindruck entsteht, der Lizenzgeber unterstütze gerade Sie oder Ihre Nutzung besonders.
- **Weitergabe unter gleichen Bedingungen** Wenn Sie das Material remixen, verändern oder anderweitig direkt darauf aufbauen, dürfen Sie Ihre Beiträge nur unter derselben Lizenz wie das Original verbreiten. 
- **Keine weiteren Einschränkungen** Sie dürfen keine zusätzlichen Klauseln oder technische Verfahren einsetzen, die anderen rechtlich irgendetwas untersagen, was die Lizenz erlaubt. 

Hinweise:
- Sie müssen sich nicht an diese Lizenz halten hinsichtlich solcher Teile des Materials, die gemeinfrei sind, oder soweit Ihre Nutzungshandlungen durch Ausnahmen und Schranken des Urheberrechts gedeckt sind.
- Es werden keine Garantien gegeben und auch keine Gewähr geleistet. Die Lizenz verschafft Ihnen möglicherweise nicht alle Erlaubnisse, die Sie für die jeweilige Nutzung brauchen. Es können beispielsweise andere Rechte wie Persönlichkeits- und Datenschutzrechte zu beachten sein, die Ihre Nutzung des Materials entsprechend beschränken.

*Dies war eine allgemeinverständliche Zusammenfassung der [Lizenz](https://creativecommons.org/licenses/by-sa/4.0/legalcode.de), die diese nicht ersetzt.*

## 15.3 Externe Links
Bitte erlauben Sie uns auch noch ein paar Wörter zu den auf dieser Seite gesetzten Links, wie sie von [eRecht24](https://www.e-recht24.de/muster-disclaimer.html) empfohlen werden:

Unser Angebot enthält Links zu externen Websites Dritter, auf deren Inhalte wir keinen Einfluss haben. Deshalb können wir für diese fremden Inhalte auch keine Gewähr übernehmen. Für die Inhalte der verlinkten Seiten ist stets der jeweilige Anbieter oder Betreiber der Seiten verantwortlich. Die verlinkten Seiten wurden zum Zeitpunkt der Verlinkung auf mögliche Rechtsverstöße überprüft. Rechtswidrige Inhalte waren zum Zeitpunkt der Verlinkung nicht erkennbar. Eine permanente inhaltliche Kontrolle der verlinkten Seiten ist jedoch ohne konkrete Anhaltspunkte einer Rechtsverletzung nicht zumutbar. Bei Bekanntwerden von Rechtsverletzungen werden wir derartige Links umgehend entfernen.
