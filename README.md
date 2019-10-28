# <img src="https://github.com/maxng07/filecrypter-gui/blob/master/avatar-pcmi.png"> FileCrypter-GUI
FileCrypt-GUI is an extension of <a href="https://github.com/maxng07/FileCrypter"> FileCrypter Program </a> offering a WebApp GUI. This allows user to use their web browser to select file for encryption and decryption with a Passphrase. The program is designed for local machine usage, and possible to be within the same Local Area Office Network, but not meant for Cloud deployment. For a typical cloud or cross network deployment, more work needs to be done including adding HTTPS support, multi CORE support for multi users. FileCrypter-GUI can be quickly extended to do that. 

As the program is designed for user's local machine usage, a lot of thought process and design for FileCrypter-GUI to be memory and CPU efficient, and user friendly. A simple HTML webpage with a form captures the essential information needed to perform encryption or decryption including, 
1. Allowing the user to select the file
2. Button to select Encryption or Decryption mode
3. New file name for the file
4. Password used to encrypt the file.
A graphical pictorial is available <a href="https://github.com/maxng07/filecrypter-gui/blob/master/tutorial/filecrypt-gui.png"> here </a>

FileCrypter-GUI uses the same cipher logic in FileCrypter program and add a WebServer layer to interface with the user's web browser. With this design, it is possible to encrypt with FileCrypter-GUI and decrypt with FileCrypter which is a CLI based program, and vice versa. Giving user full flexibility and a Local System Administrator flexibility to support the user base. And Enterprise version could be made available with more enhanced features set to fit the Enterprise's requirement.

The program uses AES-GCMSIV cipher suite with AES256 for encryption and the user's secret password is not stored within the ecrypted file. The user needs to remember the password used to perform encryption.

<h2>Usage </h2>


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

