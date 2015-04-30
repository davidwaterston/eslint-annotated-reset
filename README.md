## ESLint Annotated Reset

<a href="http://semver.org" target="_blank" alt="Semantic Versioning"><img src="https://img.shields.io/badge/semver-0.20.0-lightgrey.svg?style=flat-square"></a>
<a href="https://github.com/davidwaterston/eslint-annotated-reset/blob/master/LICENSE" target="_blank" alt="MIT License"><img src="http://img.shields.io/badge/license-MIT-blue.svg?style=flat-square"></a>
<a href="#verifying-releases" alt="Releases signed with Gnu Privacy Guard"><img src="https://img.shields.io/badge/gpg-signed-green.svg?style=flat-square"></a>
<a href="https://gitter.im/davidwaterston/eslint-annotated-reset" target="_blank" alt="Join the chat at https://gitter.im/davidwaterston/eslint-annotated-reset"><img src="https://badges.gitter.im/Join%20Chat.svg"></a>
  
'ESLint Annotated Reset' is an [ESLint](http://eslint.org) config file - .eslintrc - that contains an entry for every rule currently available. All of these rules are turned off, which means that using it in your project would result in no linting being done at all. Why use it? If you are using ESLint on a codebase for the first time you are likely to get many errors or warnings, even with only the relaxed default settings turned on. On legacy apps the number of problems reported may be overwhelming and lead to linting being abandoned before it has the chance to be adopted. By starting with _eslint-annotated-reset_ as your config you can introduce linting in a slow and methodical fashion by turning on each rule, one at a time, and fixing the, hopefully small, number of warnings generated.  
  
  
## Compatibility
This extension has been tested and confirmed to work with ESLint version 0.20.0 and later.  
The content of _eslint-annotated-reset_ will be updated to reflect changes to rules in ESLint itself. The repo version number will also be kept in sync with ESLint itself, whenever possible.
  
  
## Release History
See the [change log](https://github.com/davidwaterston/eslint-annotated-reset/blob/master/CHANGELOG.md) file for more details.
  
  
## Verifying Releases
I use <a href="http://semver.org" target="_blank" alt="Semantic Versioning">Semantic Versioning</a> to number releases. Each release is tagged with the appropriate version number and signed using <a href="https://www.gnupg.org" target="_blank" alt="Gnu Privacy Guard (GPG)">Gnu Privacy Guard (GPG)</a>. The public key used to sign releases is  
```
Name: David Waterston  
Email: david@davidwaterston.com  
Key ID: A7AD9C85  
Signature: 71A9 DC13 447A 1E4F C6EB  5D64 DE08 A991 A7AD 9C85  
```
This public key is included in the repository with a SHA1 of 16d013451476fa4a1a67d6ad4b90583e205b53b1.  
After cloning the repo, and assuming you have GPG installed correctly, you can import this key into your keychain
```
git cat-file blob pubkey | gpg --import
```
When this public key is successfully imported, you can use it to verify the integrity of any of the tagged releases of this repo
```
git tag -v v0.20.0
```
which should produce output similar to:
```
object 04f37a55784c1f3abc2cf927a935a488aa954035  
type commit  
tag v0.20.0  
tagger David Waterston <david@davidwaterston.com> 1427387056 +0000  
  
Initial commit  
  
This is just an example so don't get fixated on the details, what matters is the signature!
gpg: Signature made Thu 26 Mar 16:24:16 2015 GMT using RSA key ID A7AD9C85
gpg: Good signature from "David Waterston <david@davidwaterston.com>" [ultimate]
```
The important thing to notice here is that the RSA key ID matches mine (A7AD9C85) and the line that says that this is a good signature.  
  
The public key can further be verified by checking the details held on <a href="http://pgp.mit.edu/pks/lookup?search=david%40davidwaterston.com&op=index&fingerprint=on&exact=on" target="_blank" alt="pgp.mit.edu">pgp.mit.edu</a>.
  
  
## License
Copyright (c) 2015 David Waterston. All rights reserved.  
Distributed under an MIT license. See the [LICENSE](https://github.com/davidwaterston/eslint-annotated-reset/blob/master/LICENSE) file for more details.
