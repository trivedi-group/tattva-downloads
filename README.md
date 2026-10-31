# Tattvā downloads

This page holds the built copies of Tattvā for macOS, Windows and Linux. Tattvā is a desktop toolkit for LC-MS and GC-MS metabolomics. It runs on your own computer and your data stay there.

Tattvā needs a licence file from the Trivedi Lab before it will run. No source code is stored here.

## Before you start

1. Open the Releases page of this repository and choose the newest release.
2. Download the file that matches your computer. The file names carry the platform.

* Mac with Apple silicon (M1 or later): Tattva Mac Apple, a disk image ending in .dmg.
* Mac with an Intel processor: Tattva Mac Intel, a disk image ending in .dmg.
* Windows 10 or 11, 64 bit: Tattva Windows, a zip file ending in .zip.
* Linux, 64 bit Intel or AMD: Tattva Linux, a file ending in .tar.gz.

To find out which Mac you have, choose the Apple menu, then About This Mac. Chip means Apple silicon. Processor means Intel.

3. Optional but recommended. Check that the download is complete. Each release has a file called SHA256SUMS.txt. Compare the line for your file with the checksum on your computer.
   * Mac: open Terminal and type `shasum -a 256 ` followed by the file name.
   * Windows: open PowerShell and type `Get-FileHash ` followed by the file name.
   * Linux: open a terminal and type `sha256sum ` followed by the file name.

   The two values must be identical.

## Install on macOS

1. Double click the disk image.
2. Drag Tattva onto the Applications folder shown in the window.
3. Double click Tattva in Applications. macOS says it cannot verify the app, because Tattvā is not yet signed with an Apple developer certificate. Click Done. Do not move it to the Bin.
4. Open System Settings, choose Privacy and Security and scroll to the Security section.
5. Next to the message that Tattva was blocked, click Open Anyway. Enter your Mac password or use Touch ID, then click Open Anyway once more.

You only need to do this once for each copy of the app. On macOS 14 Sonoma or earlier there is a shorter way. Right click Tattva, choose Open, then choose Open again. If you cannot find Open Anyway, double click Tattva again first. The button appears for about an hour after a blocked attempt.

## Install on Windows

1. Unzip the download. Right click the zip file and choose Extract All.
2. Open the Tattva folder and double click Tattva.exe.
3. If a blue window says Windows protected your PC, click More info, then Run anyway. Tattvā is not yet signed with a Windows publisher certificate, so this warning is expected the first time.

Keep the whole Tattva folder together. You can move it anywhere you own, for example your Documents folder.

## Install on Linux

This Linux version is new. It has been built and tested in a Linux sandbox without a screen, so please tell the Trivedi Lab what happens on your computer. It needs a 64 bit Intel or AMD computer, a desktop session and a web browser, because Tattvā opens in your browser.

1. Move the downloaded file to a folder you own, such as your home folder.
2. Open a terminal in that folder and type `tar -xzf ` followed by the file name in quotation marks. This makes a folder called Tattva.
3. Open the folder and start Tattvā with `./"Start Tattva.sh"`.
4. If you see Permission denied, type `chmod +x "Start Tattva.sh" Tattva` and try again.

Do not move Start Tattva.sh out of the Tattva folder. It needs the program called Tattva beside it.

## First run and your licence

1. Start Tattvā. It opens in your web browser.
2. On the licence screen you see a device code for your computer, written like 1A2B-3C4D-5E6F-7A8B. Each licence is issued to one named person for one computer, so the code is needed to issue your licence.
3. Send the device code to the Trivedi Lab with your licence request. You will receive a licence file.
4. Paste the text of the licence file into the licence screen, or choose the file. Tattvā then opens.

To move your licence to a new computer, send the new device code to the Trivedi Lab and ask for a reissue.

## Updates

In Tattvā, open About and choose Check for updates. It makes one request to this page to see whether a newer release exists. On Windows and macOS it can download the update for you, after checking it against SHA256SUMS.txt. On Linux, download the new file by hand from the Releases page.

## Help

If something does not work, open About, choose Save support report and follow the steps to send the support report and developer log to the Trivedi Lab. You can also contact the Trivedi Lab through the link in the Tattvā footer.

Tattvā is created and tested by Drupad Trivedi and the Trivedi Lab.
