# chromedriver-2.31
This is a developer preview release of ChromeDriver 2.31 (presently unreleased)

Due to a ChromeDriver issue detailed here https://bugs.chromium.org/p/chromedriver/issues/detail?id=1772, version 2.30 which was released by Google has a bug present where Xvfb (X virtual frame buffer) is not present.

This is either buggy or hard to use or requires multiple processes etc. and is not good for use within containers (Docker or otherwise).

Github user taboidun has created a recipie for compiling ChromeDriver 2.31 from source (https://gist.github.com/tabiodun/e4204ab83b3b7cfd2d28b478cf441162) but it requires quite a powerful compute resource to generate the ~11mb binary.

Using ubuntu 14.04 (Trusty Tahr) on an x86 architecture with 15 Gb memory and an attached 150 Gb EBS volume (a relatively expensive machine to provision) the prerelease 2.31 binary is available.

This was compiled as of 8 July 2017, and will be out of date as soon as a commit is pushed upstream.

The official ChromeDriver 2.31 release will be available here: https://sites.google.com/a/chromium.org/chromedriver/downloads.
