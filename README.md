<p align="center"><img src="assets/pnevma-package-manager-256.png" width="128" alt="Pnevma Package Manager logo"></p>

# Pnevma Package Manager

Design box-with-lid packaging and send it straight to LightBurn. The pieces arrive at their real size, already on their
own layers. Put a logo or a repeating pattern on the lid, and see how many boxes fit on the board you buy.

- Windows 10 (version 1809) or Windows 11, 64-bit.
- Closed source. This repository holds only the downloads, the license agreement, the order terms and the notices.

## Download

**[Latest release](https://github.com/pan7266/Pnevma-Package-Generator/releases/latest)**

Version 0.5.0 fits more boxes on a board (the pieces nest by their real shape), sends the whole sheet to LightBurn,
and updates itself: **Settings → Updates → Update now**. Download 0.5.0 once; later versions install from inside the
app. The license agreement is now version 1.2, so the app asks you to accept it again.

## Install

**The single exe (simplest)**

1. Download `Pnevma-Package-Manager-0.5.0-win-x64.exe` from the release.
2. Move it to a folder you keep, such as `Documents`, and run it. The first start takes a little longer, because it
   unpacks itself.
3. The app is not code-signed yet, so Windows may say **"Windows protected your PC"**. Click **More info**, then
   **Run anyway**.

**Or the zip**

1. Download `Pnevma-Package-Manager-0.5.0-win-x64.zip`, right-click it, choose **Extract All…**, and pick a folder you
   keep. Don't run the app from inside the zip.
2. Open the `Pnevma Package Manager` folder and run `Pnevma.PackageGenerator.exe`.

There is nothing else to install: the app brings its own .NET and Windows App SDK.

## Updates

From 0.5.0 on, the app looks for a newer version on this page when it starts (at most once a day) and when you click
**Settings → Updates → Check for updates**. **Update now** downloads the new version, checks it against the release's
`SHA256SUMS.txt`, puts it in place of your copy (the same exe, or the same folder) and restarts. Your boxes, logos,
settings and licence stay as they are. The automatic check can be turned off in the same place. A copy in a folder
that needs an administrator, such as Program Files, can't update itself; download the new version here instead.

## First start: accept the agreement, sign in and get a licence

1. Read the **End User License Agreement** (it includes the privacy notice; **Διαβάστε στα Ελληνικά** shows it in
   Greek). Tick **I have read and accept…** and click **Accept and continue**. **Decline** closes the app. The app
   asks again only when the agreement changes.
2. Click **Continue with email**, or **New to Pnevma? Create an account** the first time. You sign in in your
   browser, on the Pnevma Tools page; the app never sees your password.
3. If your account has no licence yet, the app says so and opens **Contact us**. Send the message. It already holds
   your computer code, which we need to set up your licence.
4. When we tell you the licence is ready, click **Try again**.

Good to know:
- A licence works on **one computer**. To move it to a new computer, write to us and we free the seat.
- The app keeps working **offline for up to 7 days** after it last reached the licence server.
- Your settings and logos are in `%LOCALAPPDATA%\Pnevma\PackageGenerator`. To remove the app, delete the exe (or the
  extracted folder), and that folder too if you want your settings gone.

## Buying a licence

Paid licences are sold under the [Order Terms](ORDER-TERMS.txt), in English and Greek: how to order, prices and
payment, delivery, no automatic renewal, and the 14-day right of withdrawal for consumers, with a model withdrawal
form. In the app, **Settings → License and account → Order terms** opens them too.

## Check the download (optional)

Compare the file's fingerprint with `SHA256SUMS.txt` in the release. In PowerShell, in the folder with the download:

```powershell
Get-FileHash .\Pnevma-Package-Manager-0.5.0-win-x64.exe -Algorithm SHA256
```

## Support

Anastasia Pnevmatikou (Pnevma), Kountouriotou 7, 18756 Keratsini, Greece. info@pnevmagifts.gr

## License agreement and privacy

Proprietary. The [End User License Agreement](LICENSE.txt), in English and Greek, sets the terms of use. Its Part B
explains what personal data the license service keeps (your account e-mail, name and computer code, never your designs
or logos), where it is stored (the EU), what GitHub sees when the app checks for updates (your IP address and the app's
version) and your rights. Copying, redistributing, reverse engineering and using the
software for AI training are not allowed. The app includes Microsoft and other components under their own licenses:
see [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt).

---

## Ελληνικά

Το **Pnevma Package Manager** σχεδιάζει κουτιά με καπάκι και τα στέλνει κατευθείαν στο LightBurn, σε πραγματικό
μέγεθος και σε έτοιμα layers.

1. Κατεβάστε το `Pnevma-Package-Manager-0.5.0-win-x64.exe` από την
   **[τελευταία έκδοση](https://github.com/pan7266/Pnevma-Package-Generator/releases/latest)**, μετακινήστε το σε έναν
   φάκελο που κρατάτε και ανοίξτε το. Η πρώτη εκκίνηση αργεί λίγο. (Υπάρχει και zip: δεξί κλικ → **Εξαγωγή όλων…** και
   ανοίξτε το `Pnevma.PackageGenerator.exe` από τον φάκελο.)
2. Αν τα Windows δείξουν «Τα Windows προστάτευσαν τον υπολογιστή σας», πατήστε **Περισσότερες πληροφορίες** και μετά
   **Εκτέλεση οπωσδήποτε**.
3. Η πρώτη οθόνη είναι η Σύμβαση Άδειας Χρήσης Τελικού Χρήστη· το **Διαβάστε στα Ελληνικά** τη δείχνει στα Ελληνικά.
   Τσεκάρετε **I have read and accept…** και πατήστε **Accept and continue**.
4. Η επόμενη οθόνη είναι στα αγγλικά. Πατήστε **Continue with email** (ή **Create an account** την πρώτη φορά) και
   συνδεθείτε στον browser.
5. Αν δεν έχετε ακόμη άδεια, στείλτε μας το μήνυμα από το **Contact us**. Περιέχει ήδη τον κωδικό του υπολογιστή σας.
6. Όταν σας ενημερώσουμε, πατήστε **Try again**. Μετά, από **Settings → Language / Γλώσσα** επιλέξτε Ελληνικά.

Από την έκδοση 0.5.0 η εφαρμογή ενημερώνεται μόνη της: **Ρυθμίσεις → Ενημερώσεις → Ενημέρωση τώρα**. Κατεβάστε την 0.5.0
μία φορά· οι επόμενες εκδόσεις εγκαθίστανται μέσα από την εφαρμογή, χωρίς να χαθούν κουτιά, λογότυπα, ρυθμίσεις ή η άδεια.

Μία άδεια = ένας υπολογιστής. Οι όροι χρήσης και η ενημέρωση για τα προσωπικά δεδομένα βρίσκονται στο
[LICENSE.txt](LICENSE.txt) και οι όροι αγοράς στο [ORDER-TERMS.txt](ORDER-TERMS.txt). Πνευματικού Αναστασία (Pnevma),
Κουντουριώτου 7, 18756 Κερατσίνι. Επικοινωνία: info@pnevmagifts.gr
