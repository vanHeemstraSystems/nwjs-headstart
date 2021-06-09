nwjs-headstart
# NW.js - Headstart

Based on "NW.js" at https://nwjs.io/

Based on "nw.js" at https://github.com/nwjs/nw.js

```Call all Node.js modules directly from DOM/WebWorker and enable a new way of writing applications with all Web technologies.```

## 100 - Introduction

NW.js is an app runtime based on Chromium and node.js. You can write native apps in HTML and JavaScript with NW.js. It also lets you call Node.js modules directly from the DOM and enables a new way of writing native applications with all Web technologies.

## 200 - Features

- Apps written in modern HTML5, CSS3, JS and WebGL.
- Complete support for Node.js APIs and all its third party modules.
- Good performance: Node and WebKit run in the same thread: Function calls are made straightforward; objects are in the same heap and can just reference each other.
- Easy to package and distribute apps.
- Available on Linux, Mac OS X and Windows.

## 300 - Downloads

- v0.54.0: (May 26, 2021, based off of Node.js v16.1.0, Chromium 91.0.4472.77) : release notes
NOTE You might want the SDK build. Please read the release notes.

- Linux: 32bit / 64bit

- Windows: 32bit / 64bit

- Mac 10.10+: 64bit

- Use Legacy build for Win XP and early OSX.

- latest nightly build from git tip: https://dl.nwjs.io/live-build/

- Previous versions; See the mapping file for the version info in previous releases.

## 400 - Demos and real apps

You may also be interested in our [demos repository](https://github.com/zcbenz/nw-sample-apps) and the [List of apps and companies using nw.js](https://github.com/nwjs/nw.js/wiki/List-of-apps-and-companies-using-nw.js).

## 500 - Quickstart

See [README.md](./500/README.md)

## 600 - Documents
Official documentation: [http://docs.nwjs.io/](http://docs.nwjs.io/)

For more information on how to write/package/run apps, see:

- [How to run apps](https://github.com/nwjs/nw.js/wiki/How-to-run-apps)
- [How to package and distribute your apps](https://github.com/nwjs/nw.js/wiki/How-to-package-and-distribute-your-apps)
- [How to use Node.js modules in node-webkit](https://github.com/nwjs/nw.js/wiki/Using-Node-modules)

And our [Wiki](https://github.com/nwjs/nw.js/wiki) for much more.

## 700 - Community

We use the google group as our mailing list (use English only). Subscribe via nwjs-general+subscribe@googlegroups.com.

NOTE: Links to the old google group (e.g. https://groups.google.com/forum/#!msg/node-webkit/doRWZ07LgWQ/4fheV8FF8zsJ) that are no longer working can be fixed by replacing node-webkit with nwjs-general (e.g https://groups.google.com/forum/#!msg/nwjs-general/doRWZ07LgWQ/4fheV8FF8zsJ).

Issues are being tracked here on GitHub.

The source code for NW.js and the daily development spans across multiple repositories in this organization. This repository is for the purpose of issue tracking, landing page and part of the source code.

## 800 - Verifying Binaries

Starting from 0.32.0 the stable and nightly download directories contain a SHASUMS256.txt
file that lists the SHA checksums for each file available for download, as well as the
checksums for the files inside the download package.

The SHASUMS256.txt can be downloaded using `curl`.

```console
$ curl -O https://dl.nwjs.io/vx.y.z/SHASUMS256.txt
```

To check that a downloaded file matches the checksum, run
it through `sha256sum` with a command such as:

```console
$ grep nwjs-vx.y.z.tar.gz SHASUMS256.txt | sha256sum -c -
```

The stable releases (but not Nightlies) also have the GPG detached
signature of SHASUMS256.txt available as SHASUMS256.txt.asc. You can use `gpg`
to verify that SHASUMS256.txt has not been tampered with.

To verify SHASUMS256.txt has not been altered, you will first need to import
the GPG key of NW.js maintainer to create releases.
Use this command to import the key:

```console
$ gpg --keyserver pool.sks-keyservers.net --recv-keys 78680FA9E21BB40A
```
```
(Key fingerprint is 1E8B EE8D 5B0C 4CBC D6D1  9E26 7868 0FA9 E21B B40A)
```

Next, download the SHASUMS256.txt.asc for the release:

```console
$ curl -O https://dl.nwjs.io/vx.y.z/SHASUMS256.txt.asc
```

After downloading the appropriate SHASUMS256.txt and SHASUMS256.txt.asc files,
you can then use `gpg --verify SHASUMS256.txt.asc SHASUMS256.txt` to verify
that the file has been signed by an authorized member of the NW.js team.

Once verified, use the SHASUMS256.txt file to get the checksum for
the binary verification command above.

## 900 - License

`NW.js`'s code in this repo uses the MIT license, see our `LICENSE` file. To redistribute the binary, see [How to package and distribute your apps](https://github.com/nwjs/nw.js/wiki/How-to-package-and-distribute-your-apps)
