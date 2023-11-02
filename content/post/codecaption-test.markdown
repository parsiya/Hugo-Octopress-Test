---
title: "Codecaption test"
date: 2017-12-08T18:44:37-04:00
draft: false
toc: false
comments: false
categories:
- test
- category3
tags:
- codecaption
- tag3
---

{{< codecaption title="Python code highlight" lang="python" >}}
from base64 import b64encode
from binascii import unhexlify

print b64encode(unhexlify("0a0b0c0d"))
CgsMDQ==
{{< /codecaption >}}

{{< codecaption title="Go highlight" lang="go" >}}
// zlib inflate (decompress).

package main

import (
	"compress/zlib"
	"io"
	"os"
)

func main() {
	zlibFile, err := os.Open("test.zlib")
	if err != nil {
		panic(err)
	}
	defer zlibFile.Close()

	r, err := zlib.NewReader(zlibFile)
	if err != nil {
		panic(err)
	}
	defer r.Close()

	outFile, err := os.Create("out-zlib")
	if err != nil {
		panic(err)
	}
	defer outFile.Close()

	io.Copy(outFile, r)
}
{{< /codecaption >}}


Python code highlight using the Hugo internal `highlight` shortcode:

{{< highlight python >}}
from base64 import b64encode
from binascii import unhexlify

print b64encode(unhexlify("0a0b0c0d"))
CgsMDQ==
{{</highlight >}}

<!--more-->

test gist1

{{< gist parsiya 3c18b044bda63d34bdb83eddb66bee4c >}}

------

test gist2

{{< gist parsiya 423b289016de056671ed6af58e364b99 >}}

Powershell codecaption highlight:

{{< codecaption title="Hello" lang="posh" >}}
# notepad does not have an entry
$ Test-Path "HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths\notepad.exe"
False
# chrome does
$ Test-Path "HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths\chrome.exe"
True
{{< /codecaption >}}

Indented code block:

    # notepad does not have an entry
    $ Test-Path "HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths\notepad.exe"
    False
    # chrome does
    $ Test-Path "HKLM:\SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths\chrome.exe"
    True

