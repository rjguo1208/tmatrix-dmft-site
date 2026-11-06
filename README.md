# tmatrix-dmft-site

Password-protected project website, served by GitHub Pages from this repository.

Every page here is an encrypted shell: the page title and body are one AES-256-GCM ciphertext, and the key
is derived in the visitor's browser from the access code with PBKDF2-HMAC-SHA256 (1.2 million iterations).
Nothing is sent to a server. The access code is not stored in this repository. The pages are generated from
a private source repository; do not edit the HTML files here by hand.

`assets/katex/` is KaTeX (MIT licence, see `assets/katex/LICENSE`); `assets/style.css` is the site stylesheet.

A short numeric code keeps casual visitors out; it is not strong confidentiality, because anyone who downloads
a page can try codes offline.
