# <img src="https://github.com/maxng07/filecrypter-gui/blob/master/avatar-pcmi.png"> FileCrypter-GUI
FileCrypter-GUI is an extension of <a href="https://github.com/maxng07/FileCrypter"> FileCrypter Program </a> offering a WebApp GUI. This allows user to use their web browser to select file for encryption and decryption with a Passphrase of their choice. The program is designed for user's local machine usage, and also possible within the small office Local Area Network. However, it is not recommended for Cloud deployment outside their premise. For a typical cloud or cross network deployment, more work needs to be done including adding HTTPS support, multi CORE support for multi users. FileCrypter-GUI can be quickly extended to do that. 

As the program is designed to be used on user's local machine, a lot of thought processes and designs are considered on FileCrypter-GUI to be memory and CPU efficient, and user friendliness. A simple HTML webpage with a form captures the essential information needed to perform encryption or decryption including, 
1. Allowing the user to select the file
2. Button to select Encryption or Decryption mode
3. New file name for the file
4. Password used to encrypt the file. <br>

A graphical pictorial of the html page is shown below. For simplicity, this freeware today does not offer HTTPS as its meant for local machine usage or Small Office network. An Enterprise version with more features can be made available, please contact the author.

# Overview
FileCrypter-GUI uses the same cipher logic method used in <a href="https://github.com/maxng07/FileCrypter"> FileCrypter program </a> and add a WebServer layer. This allows the user to use their web browser they are familiar with to interact with the encryption program. With this design, it is possible to encrypt with FileCrypter-GUI and decrypt with FileCrypter CLI, and vice versa. Giving user full flexibility and the Local System Administrator flexibility to support their office user base. And Enterprise version could be made available with more enhanced features set to fit the Enterprise's requirement.

The program uses AES-GCMSIV cipher suite with AES256 for encryption and the user's secret password is not stored within the encrypted file. The user needs to remember the password used to perform encryption on their files.

<h2>Usage </h2>
1. Download the package of their choice, Windows or MAC OSX from <a href="https://github.com/maxng07/filecrypter-gui/releases"> here </a> <br>
2. Create a Directory or Folder, and place the package there. Uncompressed or UnZip the package using WinZip (for Windows). For MAC, OSX automatically unzip when you download the zipped package. <br>
3. The Zipped package contains 3 files; Indexfc.html, config.json and Filecrypter program. You will need all 3 files to run. <br>
4. Config.json sets the basic configuration, you can edit it using a text editor. The default settings are pre-configured and you do not need to change it. If there is a need, you can edit config.json to change IP address and TCP port. </br>
5. Launch Filecrypter program by double clicking on it in Windows, for MAC clicking on the program for Finder windows works too. <br>
6. Launch your web browser, and use this in the address bar http://127.0.0.1:8888 and enter. <br>
You should see a webpage like this. <p>
<img src="https://github.com/maxng07/filecrypter-gui/blob/master/tutorial/filecrypt-gui.png">

An animated tutorial has been created if you need help using the Web Page. You can refer it <a href="https://github.com/maxng07/filecrypter-gui/blob/master/tutorial/FileCrypt-mov.gif"> here. </a>

<h2> Performance </h2>
Encryption test has been done on old i7 CORE MAC. A 2.5MB file took about approx 1s to complete encryption and a 10MB file took about less than 5s to complete encryption.

<h2>Licensing </h2>
 All RIGHTS RESERVED.
 
 Filecrypt-GUI also uses a GO package for AES-GCMSIV which has a copyright license as part of BoringSSL. The copyright notice as is below
<p>

/* Copyright (c) 2017, Google Inc.
 *
 * This code was written to support development of BoringSSL and thus is
 * considered part of BoringSSL and under the same license.
 *
 * Permission to use, copy, modify, and/or distribute this software for any
 * purpose with or without fee is hereby granted, provided that the above
 * copyright notice and this permission notice appear in all copies.
 *
 * THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 * WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 * MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY
 * SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 * WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION
 * OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN
 * CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE. */ 

