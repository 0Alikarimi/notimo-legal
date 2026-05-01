# Datenschutzerklärung — Notimo

**Stand:** 25. April 2026
**App:** Notimo (Klavier-Lern-App für iOS)
**Anbieter:** Ali Karimi
**Kontakt:** notimoapp@gmail.com

---

## Kurzfassung

Notimo ist eine Klavier-Lern-App. Wir betreiben **keine eigenen Server**.
Wir verkaufen, teilen oder versenden deine Daten an niemanden. Wir nutzen
**kein Tracking, keine Analytics, keine Werbung**. Alles, was du in der
App machst, bleibt entweder auf deinem Gerät oder in deinem privaten
iCloud-Account, auf den nur du Zugriff hast.

Das Einzige, was wir je „sehen", ist die opake Apple-Benutzer-ID, die
Apple uns beim Sign-in liefert — und die liegt im iOS-Keychain auf deinem
eigenen Gerät. Wir lesen sie nicht aus, schicken sie nirgendwohin und
verknüpfen sie mit nichts.

---

## 1. Wer wir sind

Notimo wird von Ali Karimi als unabhängige iOS-Indie-App entwickelt. Es
gibt keine Firma, keine Investoren, kein Marketing-Team und vor allem
**keinen eigenen Backend-Server**. Die App kommuniziert mit genau zwei
Stellen:

1. **Lokaler Speicher deines Geräts** (UserDefaults / Keychain / App-Sandbox)
2. **Dein eigener privater iCloud-Account** (Apple-Server, deine Apple-ID)

Mehr nicht. Es gibt keine Notimo-Cloud, keine Notimo-Analytics, keine
Datenhändler.

---

## 2. Welche Daten wir verarbeiten

Wir listen alle Kategorien auf, die Apples Privacy-Framework kennt — auch
wenn die Daten dein Gerät nie verlassen. Lieber transparent als knapp.

### 2.1 Sign in with Apple — Apple-Benutzer-ID

Wenn du auf „Mit Apple anmelden" tippst, gibt Apple der App eine **opake
Benutzer-ID**. Das ist eine lange Folge zufälliger Zeichen, die dich
*nur dieser App* eindeutig zuordnet. Es ist NICHT deine Apple-ID, NICHT
deine E-Mail, NICHT dein Name. Sie kann von uns oder Dritten nicht in
deine echte Apple-ID zurückübersetzt werden.

- **Wo gespeichert:** iOS-Keychain auf deinem Gerät (Apples sicherer Speicher)
- **Wofür:** um zu erkennen „das ist derselbe User wie letztes Mal" und
  um deinen iCloud-Sync deinem Konto zuzuordnen
- **Niemals weitergegeben an:** irgendjemanden. Punkt.

### 2.2 E-Mail und Name — nur, wenn Apple sie liefert

Beim allerersten Sign-in kann Apple der App optional deine E-Mail und
deinen Namen geben — aber nur, wenn du es erlaubst. Du kannst wählen:

- **„E-Mail verbergen"** → Apple liefert nur eine Relay-Adresse, die an
  dich weiterleitet. Wir sehen deine echte E-Mail nicht.
- **Name/E-Mail nicht teilen** → wir bekommen nichts.

Falls Apple eine E-Mail oder einen Namen mitliefert, speichern wir das
lokal auf deinem Gerät (UserDefaults), nur um es im Account-Bereich der
Einstellungen anzuzeigen. Wir schreiben dir keine E-Mails. Es gibt keinen
Newsletter. Wir geben das nicht weiter.

### 2.3 Dein Lernfortschritt (XP, Streak, Erfolge, Einstellungen)

Deine tägliche Streak, XP, abgeschlossenen Lektionen, Einstellungen
(Sprache, Theme, Übungsziel, Metronom-Sound usw.) und identifizierten
Schwachnoten werden gespeichert:

- **Lokal** auf deinem Gerät in UserDefaults
- **In deinem privaten iCloud-Account** über Apples iCloud-Key-Value-Store
  und CloudKit, damit derselbe Fortschritt auf allen Geräten unter
  derselben Apple-ID erscheint

Diese Daten werden von Apple bei der Übertragung und Speicherung
verschlüsselt. **Wir haben keinerlei Zugriff darauf.** Nur du, mit deiner
Apple-ID angemeldet, kannst sie lesen.

### 2.4 Importierte Songs und SoundFonts

Wenn du MusicXML-/.mxl-Dateien oder SoundFont-Dateien (.sf2) importierst,
liegen sie in der App-Sandbox auf deinem Gerät. Dateinamen werden — wie
bei jeder iOS-App — in dein iCloud-Drive synchronisiert, falls aktiviert.
Wir lesen die Dateien zu keinem anderen Zweck als Wiedergabe und Anzeige
in der App.

### 2.5 Mikrofon (optional)

Notimo kann gespielte Noten an einem akustischen Klavier per Mikrofon
erkennen. Das Audio wird in Echtzeit ausgewertet und **nie aufgezeichnet,
gespeichert oder versendet**. Nach der Erkennung wird der Audio-Sample
verworfen. Diese Funktion ist nur aktiv, wenn du sie unter Einstellungen
→ „Mikrofon-Erkennung" explizit einschaltest.

### 2.6 Was wir NICHT erheben

- ❌ Keine Adresse, Telefonnummer (jenseits dessen, was Apple optional liefert)
- ❌ Keine Standortdaten
- ❌ Keine Werbe-IDs (IDFA)
- ❌ Kein Browsing-/Nutzungsverlauf außerhalb der App
- ❌ Kein Device-Fingerprinting
- ❌ Keine Crash-Reports an Dritte (nur an Apple via Xcode, falls aktiviert)
- ❌ Keine Drittanbieter-SDKs (kein Firebase, Mixpanel, Amplitude, Adjust,
  Branch, Facebook SDK, Google Analytics o.ä.)
- ❌ Keine Zahlungsdaten — wir nutzen Apples StoreKit, Apple verarbeitet
  alle Kaufdaten; wir sehen lokal nur „Pro aktiv: ja/nein"

---

## 3. Tracking

**Wir tracken dich nicht.** Nicht in der App, nicht über Apps hinweg,
nicht im Web. Das Privacy Manifest deklariert `NSPrivacyTracking = false`,
und es sind null Tracking-Domains in der App-Binary.

---

## 4. Drittanbieter

Wir nutzen genau zwei Apple-Dienste:

| Dienst | Wofür | Apples Datenschutz |
|---|---|---|
| **Sign in with Apple** | Anmeldung | [apple.com/legal](https://www.apple.com/legal/privacy/data/de/sign-in-with-apple/) |
| **iCloud (KV-Store + CloudKit)** | Sync zwischen deinen Geräten | [apple.com/legal/privacy/icloud](https://www.apple.com/legal/privacy/data/de/icloud/) |

Beide Dienste werden von Apple Inc. betrieben und unterliegen Apples
Datenschutzrichtlinien. Notimo selbst sieht die Daten, die Apple für dich
speichert, nie.

Wir nutzen **keine** Nicht-Apple-Drittanbieter-Dienste.

---

## 5. Kinder

Notimo ist für alle Altersgruppen geeignet, aber Sign in with Apple hat
ein von Apple festgelegtes Mindestalter (in den meisten Regionen 13).
Jüngere Kinder sollten Apples Familienfreigabe nutzen. Wir erheben
wissentlich keine Daten von Kindern unter 13 — wir erheben generell kaum
Daten — und die App funktioniert vollständig auch ohne Anmeldung für
Nutzer, die keinen Cloud-Sync wollen.

---

## 6. Deine Rechte

Du kannst jederzeit:

- **Deine Daten einsehen:** App → Einstellungen → Account. Deine Apple-ID
  liegt im iOS-Keychain (mit Apples Standard-Entwickler-Tools sichtbar).
- **Sync stoppen:** in iOS-Einstellungen → [Dein Name] → iCloud → Apps
  → Notimo deaktivieren.
- **Abmelden:** Einstellungen → Account → Abmelden (in der App).
- **Account löschen:** Einstellungen → Account → Account löschen. Das
  entfernt sofort:
  - Deine Apple-Benutzer-ID aus dem Keychain des Geräts
  - Deinen lokal zwischengespeicherten Fortschritt
  - Deine iCloud-Key-Value-Store-Daten für Notimo
- **Sign in with Apple vollständig widerrufen:** weil wir keine Server
  betreiben, können wir die Apple-Autorisierung nicht serverseitig
  widerrufen. Das machst du selbst: iOS-Einstellungen → [Dein Name] →
  Mit Apple anmelden → Notimo → „Apple-ID nicht mehr verwenden". Die App
  zeigt dir nach dem Löschen einen Hinweis darauf.

Nach DSGVO (Art. 15–22) hast du zusätzlich das Recht auf Auskunft,
Berichtigung, Löschung, Einschränkung der Verarbeitung, Datenübertragbarkeit
und Widerspruch sowie das Recht auf Beschwerde bei einer Aufsichtsbehörde.
Da wir keine personenbezogenen Daten auf eigenen Servern verarbeiten,
laufen diese Rechte praktisch über die obigen In-App-Schritte und Apples
iCloud-Datenschutz.

---

## 7. Speicherdauer

- **Auf deinem Gerät:** bis du dich abmeldest, den Account in der App
  löschst oder die App deinstallierst.
- **In deinem iCloud:** unterliegt Apples iCloud-Aufbewahrungsregeln und
  deinen eigenen Apple-Einstellungen. Beim Löschen deines Notimo-Accounts
  in der App versuchen wir, die von uns geschriebenen iCloud-Key-Value-
  Einträge zu löschen.

---

## 8. Sicherheit

- Apple-Benutzer-ID im iOS-Keychain mit
  `kSecAttrAccessibleAfterFirstUnlock` — dieselbe Schutzklasse, die alle
  großen iOS-Apps für sensible Credentials nutzen.
- Daten in iCloud sind bei Übertragung (TLS) und Speicherung von Apple
  verschlüsselt.
- Die App nutzt Anti-Debug-Schutz in Release-Builds.
- Wir speichern weder Passwörter noch Kreditkartendaten — Apple
  übernimmt Anmeldung und Bezahlung vollständig.

---

## 9. Internationale Nutzer

Da es keinen Notimo-Server gibt, verlassen deine Daten weder dein Gerät
noch deine eigene Apple-iCloud-Region. Apple speichert iCloud-Daten gemäß
seinen iCloud-AGB in deiner Region.

---

## 10. Änderungen dieser Erklärung

Falls sich je etwas an den erhobenen Daten ändert (z.B. neues Feature mit
neuen Berechtigungen), aktualisieren wir diese Seite und das Datum oben.
Bei wesentlichen Änderungen (z.B. Einführung jeglicher Analytics oder
eines Backend-Servers) zeigt die App einen klaren In-App-Hinweis und
fragt erneut nach Einverständnis.

---

## 11. Verantwortlicher i.S.d. DSGVO

Verantwortlicher i.S.d. Art. 4 Nr. 7 DSGVO:

**Ali Karimi**
Trompeterstr. 49a
40764 Langenfeld
Deutschland
E-Mail: notimoapp@gmail.com

---

## 12. Kontakt

Fragen zum Datenschutz? E-Mail an **notimoapp@gmail.com**.

---

*Notimo ist ein unabhängiges Indie-Projekt. Keine eigenen Server. Kein
Tracking. Kein Datenhandel. Keine Überraschungen.*
