# Comparing `tmp/cryptography-42.0.5.tar.gz` & `tmp/cryptography-42.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptography-42.0.5.tar", last modified: Sat Feb 24 01:05:06 2024, max compression
+gzip compressed data, was "cryptography-42.0.6.tar", last modified: Sat May  4 15:23:05 2024, max compression
```

## Comparing `cryptography-42.0.5.tar` & `cryptography-42.0.6.tar`

### file list

```diff
@@ -1,471 +1,471 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.359998 cryptography-42.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    98530 2024-02-24 01:04:55.000000 cryptography-42.0.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-24 01:04:55.000000 cryptography-42.0.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-24 01:04:55.000000 cryptography-42.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-02-24 01:04:55.000000 cryptography-42.0.5/LICENSE.APACHE
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-02-24 01:04:55.000000 cryptography-42.0.5/LICENSE.BSD
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-24 01:04:55.000000 cryptography-42.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-02-24 01:05:06.359998 cryptography-42.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-02-24 01:04:55.000000 cryptography-42.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.291998 cryptography-42.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.291998 cryptography-42.0.5/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/_ext/cryptography-docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/_ext/linkcode_res.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.291998 cryptography-42.0.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/api-stability.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/community.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.291998 cryptography-42.0.5/docs/development/
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/c-bindings.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/aes-192-gcm-siv/
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/aes-192-gcm-siv/generate_aes192gcmsiv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/aes-192-gcm-siv/verify-aes192gcmsiv/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/aes-192-gcm-siv/verify-aes192gcmsiv/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/aes-192-gcm-siv/verify-aes192gcmsiv/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/aes-192-gcm-siv/verify-aes192gcmsiv/src/main.rs
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/aes-192-gcm-siv.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/arc4/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/arc4/generate_arc4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/arc4/verify_arc4.go
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/arc4.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/cast5/
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/cast5/generate_cast5.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/cast5/verify_cast5.go
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/cast5.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/chacha20/
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/chacha20/generate_chacha20_overflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/chacha20/verify_chacha20_overflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/chacha20.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/hkdf/
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/hkdf/generate_hkdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/hkdf/verify_hkdf.go
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/hkdf.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/idea/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/idea/generate_idea.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/idea/verify_idea.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/idea.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/rsa-oaep-sha2/
--rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/rsa-oaep-sha2.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/secp256k1/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/secp256k1/generate_secp256k1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/secp256k1/verify_secp256k1.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/secp256k1.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.295998 cryptography-42.0.5/docs/development/custom-vectors/seed/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/seed/generate_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/seed/verify_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/custom-vectors/seed.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/reviewing-patches.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/submitting-patches.rst
--rw-r--r--   0 runner    (1001) docker     (127)    61328 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/development/test-vectors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/doing-a-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/fernet.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.279998 cryptography-42.0.5/docs/hazmat/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.299998 cryptography-42.0.5/docs/hazmat/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/aead.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.299998 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/
--rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/dh.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/dsa.rst
--rw-r--r--   0 runner    (1001) docker     (127)    28444 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/ec.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/ed25519.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/ed448.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    27318 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/rsa.rst
--rw-r--r--   0 runner    (1001) docker     (127)    56786 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/serialization.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/x25519.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/asymmetric/x448.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/constant-time.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9405 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/cryptographic-hashes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    44279 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/key-derivation-functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/keywrap.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.299998 cryptography-42.0.5/docs/hazmat/primitives/mac/
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/mac/cmac.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/mac/hmac.rst
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/mac/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/mac/poly1305.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/padding.rst
--rw-r--r--   0 runner    (1001) docker     (127)    33086 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/symmetric-encryption.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/hazmat/primitives/twofactor.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/openssl.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/random-numbers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/security.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/spelling_wordlist.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.303998 cryptography-42.0.5/docs/x509/
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/x509/certificate-transparency.rst
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/x509/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30012 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/x509/ocsp.rst
--rw-r--r--   0 runner    (1001) docker     (127)   134346 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/x509/reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/x509/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-02-24 01:04:55.000000 cryptography-42.0.5/docs/x509/verification.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-02-24 01:04:55.000000 cryptography-42.0.5/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-02-24 01:04:55.000000 cryptography-42.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 01:05:06.359998 cryptography-42.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.283998 cryptography-42.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.303998 cryptography-42.0.5/src/_cffi_src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/build_openssl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.307998 cryptography-42.0.5/src/_cffi_src/openssl/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/asn1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/bignum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/bio.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/cryptography.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/dh.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/dsa.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/ec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/err.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/evp.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/nid.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/opensslv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/pem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/pkcs12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/rand.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/x509.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/x509_vfy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/x509name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/openssl/x509v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/_cffi_src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.307998 cryptography-42.0.5/src/cryptography/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/fernet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.311998 cryptography-42.0.5/src/cryptography/hazmat/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/_oid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.311998 cryptography-42.0.5/src/cryptography/hazmat/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.311998 cryptography-42.0.5/src/cryptography/hazmat/backends/openssl/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/backends/openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/backends/openssl/aead.py
--rw-r--r--   0 runner    (1001) docker     (127)    32966 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/backends/openssl/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/backends/openssl/ciphers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/backends/openssl/decode_asn1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.311998 cryptography-42.0.5/src/cryptography/hazmat/bindings/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.311998 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/_openssl.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/asn1.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/ocsp.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.315998 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/aead.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/cmac.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/dh.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/ec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/keys.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/rsa.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/x448.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/pkcs7.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/x509.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.315998 cryptography-42.0.5/src/cryptography/hazmat/bindings/openssl/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/openssl/_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/bindings/openssl/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.315998 cryptography-42.0.5/src/cryptography/hazmat/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/_asymmetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/_cipheralgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.319998 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/dh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/dsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/ec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/ed25519.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/ed448.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/padding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/x25519.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/x448.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.319998 cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/aead.py
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/cmac.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/constant_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/hashes.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/hmac.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.319998 cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/concatkdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/kbkdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/scrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/x963kdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/keywrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/padding.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/poly1305.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.323998 cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/pkcs12.py
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (127)    50051 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.323998 cryptography-42.0.5/src/cryptography/hazmat/primitives/twofactor/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/twofactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/twofactor/hotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/hazmat/primitives/twofactor/totp.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.323998 cryptography-42.0.5/src/cryptography/x509/
--rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36933 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/x509/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/x509/certificate_transparency.py
--rw-r--r--   0 runner    (1001) docker     (127)    66345 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/x509/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/x509/general_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/x509/name.py
--rw-r--r--   0 runner    (1001) docker     (127)    18126 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/x509/ocsp.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/x509/oid.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/cryptography/x509/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.359998 cryptography-42.0.5/src/cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-02-24 01:05:06.000000 cryptography-42.0.5/src/cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-02-24 01:05:06.000000 cryptography-42.0.5/src/cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 01:05:06.000000 cryptography-42.0.5/src/cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 01:05:06.000000 cryptography-42.0.5/src/cryptography.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-24 01:05:06.000000 cryptography-42.0.5/src/cryptography.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-24 01:05:06.000000 cryptography-42.0.5/src/cryptography.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.323998 cryptography-42.0.5/src/rust/
--rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.323998 cryptography-42.0.5/src/rust/cryptography-cffi/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-cffi/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-cffi/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.323998 cryptography-42.0.5/src/rust/cryptography-cffi/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-cffi/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.327998 cryptography-42.0.5/src/rust/cryptography-key-parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-key-parsing/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-key-parsing/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.327998 cryptography-42.0.5/src/rust/cryptography-key-parsing/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-key-parsing/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-key-parsing/src/rsa.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-key-parsing/src/spki.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.327998 cryptography-42.0.5/src/rust/cryptography-openssl/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-openssl/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-openssl/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.327998 cryptography-42.0.5/src/rust/cryptography-openssl/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-openssl/src/aead.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-openssl/src/cmac.rs
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-openssl/src/fips.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-openssl/src/hmac.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-openssl/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-openssl/src/poly1305.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.327998 cryptography-42.0.5/src/rust/cryptography-x509/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.331998 cryptography-42.0.5/src/rust/cryptography-x509/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/certificate.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15429 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/common.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/crl.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/csr.rs
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/extensions.rs
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/name.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/ocsp_req.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/ocsp_resp.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/oid.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509/src/pkcs7.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.327998 cryptography-42.0.5/src/rust/cryptography-x509-verification/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509-verification/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.327998 cryptography-42.0.5/src/rust/cryptography-x509-verification/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509-verification/src/certificate.rs
--rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509-verification/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509-verification/src/ops.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.327998 cryptography-42.0.5/src/rust/cryptography-x509-verification/src/policy/
--rw-r--r--   0 runner    (1001) docker     (127)    27310 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509-verification/src/policy/extension.rs
--rw-r--r--   0 runner    (1001) docker     (127)    31630 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509-verification/src/policy/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509-verification/src/trust_store.rs
--rw-r--r--   0 runner    (1001) docker     (127)    23407 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/cryptography-x509-verification/src/types.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.331998 cryptography-42.0.5/src/rust/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/asn1.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.335998 cryptography-42.0.5/src/rust/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)    27626 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/aead.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/cipher_registry.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/cmac.rs
--rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/dh.rs
--rw-r--r--   0 runner    (1001) docker     (127)    15169 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/dsa.rs
--rw-r--r--   0 runner    (1001) docker     (127)    22457 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/ec.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/ed25519.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/ed448.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/hashes.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/hmac.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/kdf.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/keys.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/poly1305.rs
--rw-r--r--   0 runner    (1001) docker     (127)    27628 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/rsa.rs
--rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/x25519.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/backend/x448.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/buf.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/exceptions.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4754 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/oid.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/padding.rs
--rw-r--r--   0 runner    (1001) docker     (127)    18084 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/pkcs7.rs
--rw-r--r--   0 runner    (1001) docker     (127)    21412 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/types.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.339998 cryptography-42.0.5/src/rust/src/x509/
--rw-r--r--   0 runner    (1001) docker     (127)    34292 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/certificate.rs
--rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/common.rs
--rw-r--r--   0 runner    (1001) docker     (127)    24301 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/crl.rs
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/csr.rs
--rw-r--r--   0 runner    (1001) docker     (127)    20006 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/extensions.rs
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/mod.rs
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/ocsp.rs
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/ocsp_req.rs
--rw-r--r--   0 runner    (1001) docker     (127)    29823 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/ocsp_resp.rs
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/sct.rs
--rw-r--r--   0 runner    (1001) docker     (127)    25833 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/sign.rs
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-02-24 01:04:55.000000 cryptography-42.0.5/src/rust/src/x509/verify.rs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.339998 cryptography-42.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.339998 cryptography-42.0.5/tests/bench/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/bench/test_aead.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/bench/test_ec_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/bench/test_hashes.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/bench/test_hmac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/bench/test_x509.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/deprecated_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/doubles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.339998 cryptography-42.0.5/tests/hazmat/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.343998 cryptography-42.0.5/tests/hazmat/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/backends/test_openssl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.343998 cryptography-42.0.5/tests/hazmat/bindings/
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/bindings/test_openssl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.351998 cryptography-42.0.5/tests/hazmat/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/fixtures_dh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/fixtures_dsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/fixtures_ec.py
--rw-r--r--   0 runner    (1001) docker     (127)    29306 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/fixtures_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_3des.py
--rw-r--r--   0 runner    (1001) docker     (127)    34423 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_aead.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_aes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_aes_gcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_arc4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_asym_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_camellia.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_cast5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_chacha20.py
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_ciphers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_cmac.py
--rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_concatkdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_constant_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    36388 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_dh.py
--rw-r--r--   0 runner    (1001) docker     (127)    39026 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_dsa.py
--rw-r--r--   0 runner    (1001) docker     (127)    50088 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_ed25519.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_ed448.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_hash_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_hashes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_hkdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_hkdf_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_hmac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_hmac_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_idea.py
--rw-r--r--   0 runner    (1001) docker     (127)    26335 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_kbkdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_kbkdf_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_keywrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_padding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_pbkdf2hmac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    34291 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_pkcs12.py
--rw-r--r--   0 runner    (1001) docker     (127)    35254 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_poly1305.py
--rw-r--r--   0 runner    (1001) docker     (127)   100702 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_scrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)    55602 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)    71151 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_x25519.py
--rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_x448.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_x963_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/test_x963kdf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.351998 cryptography-42.0.5/tests/hazmat/primitives/twofactor/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/twofactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/twofactor/test_hotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/twofactor/test_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)    17277 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/hazmat/test_oid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/test_cryptography_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/test_fernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)   188472 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/test_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    29808 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.355998 cryptography-42.0.5/tests/wycheproof/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_aes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_chacha20poly1305.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_cmac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_dsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_ecdh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_eddsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_hkdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_hmac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_keywrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_x25519.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/test_x448.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/wycheproof/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.355998 cryptography-42.0.5/tests/x509/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/x509/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/x509/test_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    55544 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/x509/test_ocsp.py
--rw-r--r--   0 runner    (1001) docker     (127)   252838 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/x509/test_x509.py
--rw-r--r--   0 runner    (1001) docker     (127)    35375 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/x509/test_x509_crlbuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)   218761 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/x509/test_x509_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/x509/test_x509_revokedcertbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 01:05:06.359998 cryptography-42.0.5/tests/x509/verification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/x509/verification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/x509/verification/test_limbo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-02-24 01:04:55.000000 cryptography-42.0.5/tests/x509/verification/test_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.152526 cryptography-42.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    98633 2024-05-04 15:22:57.000000 cryptography-42.0.6/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-04 15:22:57.000000 cryptography-42.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-04 15:22:57.000000 cryptography-42.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-05-04 15:22:57.000000 cryptography-42.0.6/LICENSE.APACHE
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-04 15:22:57.000000 cryptography-42.0.6/LICENSE.BSD
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-04 15:22:57.000000 cryptography-42.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-05-04 15:23:05.152526 cryptography-42.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-04 15:22:57.000000 cryptography-42.0.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.080525 cryptography-42.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.080525 cryptography-42.0.6/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/_ext/cryptography-docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/_ext/linkcode_res.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.080525 cryptography-42.0.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/api-stability.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/community.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.080525 cryptography-42.0.6/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/c-bindings.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.084525 cryptography-42.0.6/docs/development/custom-vectors/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.084525 cryptography-42.0.6/docs/development/custom-vectors/aes-192-gcm-siv/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/aes-192-gcm-siv/generate_aes192gcmsiv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.084525 cryptography-42.0.6/docs/development/custom-vectors/aes-192-gcm-siv/verify-aes192gcmsiv/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/aes-192-gcm-siv/verify-aes192gcmsiv/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.084525 cryptography-42.0.6/docs/development/custom-vectors/aes-192-gcm-siv/verify-aes192gcmsiv/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/aes-192-gcm-siv/verify-aes192gcmsiv/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/aes-192-gcm-siv.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.084525 cryptography-42.0.6/docs/development/custom-vectors/arc4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/arc4/generate_arc4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/arc4/verify_arc4.go
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/arc4.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.084525 cryptography-42.0.6/docs/development/custom-vectors/cast5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/cast5/generate_cast5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/cast5/verify_cast5.go
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/cast5.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.084525 cryptography-42.0.6/docs/development/custom-vectors/chacha20/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/chacha20/generate_chacha20_overflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/chacha20/verify_chacha20_overflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/chacha20.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.084525 cryptography-42.0.6/docs/development/custom-vectors/hkdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/hkdf/generate_hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/hkdf/verify_hkdf.go
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/hkdf.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.084525 cryptography-42.0.6/docs/development/custom-vectors/idea/
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/idea/generate_idea.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/idea/verify_idea.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/idea.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.088525 cryptography-42.0.6/docs/development/custom-vectors/rsa-oaep-sha2/
+-rw-r--r--   0 runner    (1001) docker     (127)    14456 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/rsa-oaep-sha2.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.088525 cryptography-42.0.6/docs/development/custom-vectors/secp256k1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/secp256k1/generate_secp256k1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/secp256k1/verify_secp256k1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/secp256k1.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.088525 cryptography-42.0.6/docs/development/custom-vectors/seed/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/seed/generate_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/seed/verify_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/custom-vectors/seed.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/reviewing-patches.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/submitting-patches.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    61328 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/development/test-vectors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/doing-a-release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11665 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/fernet.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.068524 cryptography-42.0.6/docs/hazmat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.088525 cryptography-42.0.6/docs/hazmat/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/aead.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.092525 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/
+-rw-r--r--   0 runner    (1001) docker     (127)    11892 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/dh.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12502 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/dsa.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    28444 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/ec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/ed25519.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/ed448.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    27318 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/rsa.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    56786 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/serialization.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/x25519.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/asymmetric/x448.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/constant-time.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9405 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/cryptographic-hashes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    44279 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/key-derivation-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/keywrap.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.092525 cryptography-42.0.6/docs/hazmat/primitives/mac/
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/mac/cmac.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/mac/hmac.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/mac/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/mac/poly1305.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/padding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    33086 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/symmetric-encryption.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/hazmat/primitives/twofactor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/openssl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/random-numbers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/security.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/spelling_wordlist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.092525 cryptography-42.0.6/docs/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/x509/certificate-transparency.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/x509/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    30012 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/x509/ocsp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   134346 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/x509/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/x509/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-05-04 15:22:57.000000 cryptography-42.0.6/docs/x509/verification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-05-04 15:22:57.000000 cryptography-42.0.6/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-04 15:22:57.000000 cryptography-42.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 15:23:05.152526 cryptography-42.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.072524 cryptography-42.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.092525 cryptography-42.0.6/src/_cffi_src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/build_openssl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.100525 cryptography-42.0.6/src/_cffi_src/openssl/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/asn1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/bignum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/bio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/dh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/dsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/ec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/err.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/evp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/nid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/opensslv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/pem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/pkcs12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6645 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/x509.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/x509_vfy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/x509name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/openssl/x509v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/_cffi_src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.100525 cryptography-42.0.6/src/cryptography/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/fernet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.100525 cryptography-42.0.6/src/cryptography/hazmat/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/_oid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.100525 cryptography-42.0.6/src/cryptography/hazmat/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.104525 cryptography-42.0.6/src/cryptography/hazmat/backends/openssl/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/backends/openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/backends/openssl/aead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32654 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/backends/openssl/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/backends/openssl/ciphers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/backends/openssl/decode_asn1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.104525 cryptography-42.0.6/src/cryptography/hazmat/bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.104525 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/_openssl.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/asn1.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/ocsp.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.108525 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/aead.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/cmac.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/dh.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/ec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/keys.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/rsa.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/x448.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/pkcs7.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/x509.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.108525 cryptography-42.0.6/src/cryptography/hazmat/bindings/openssl/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/openssl/_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/bindings/openssl/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.108525 cryptography-42.0.6/src/cryptography/hazmat/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/_asymmetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/_cipheralgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.112525 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/dh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/dsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/ec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/ed448.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/x25519.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/x448.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.112525 cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/aead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/cmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/constant_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/hmac.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.112525 cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/concatkdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/kbkdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/x963kdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/keywrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/poly1305.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.112525 cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/pkcs12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50051 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.116525 cryptography-42.0.6/src/cryptography/hazmat/primitives/twofactor/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/twofactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/twofactor/hotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/hazmat/primitives/twofactor/totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.116525 cryptography-42.0.6/src/cryptography/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36933 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/x509/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/x509/certificate_transparency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66345 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/x509/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/x509/general_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/x509/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18126 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/x509/ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/x509/oid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/cryptography/x509/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.152526 cryptography-42.0.6/src/cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5268 2024-05-04 15:23:05.000000 cryptography-42.0.6/src/cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15454 2024-05-04 15:23:05.000000 cryptography-42.0.6/src/cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:23:05.000000 cryptography-42.0.6/src/cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 15:23:04.000000 cryptography-42.0.6/src/cryptography.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-04 15:23:05.000000 cryptography-42.0.6/src/cryptography.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 15:23:05.000000 cryptography-42.0.6/src/cryptography.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.116525 cryptography-42.0.6/src/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.116525 cryptography-42.0.6/src/rust/cryptography-cffi/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-cffi/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-cffi/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.116525 cryptography-42.0.6/src/rust/cryptography-cffi/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-cffi/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.116525 cryptography-42.0.6/src/rust/cryptography-key-parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-key-parsing/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-key-parsing/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.120525 cryptography-42.0.6/src/rust/cryptography-key-parsing/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-key-parsing/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-key-parsing/src/rsa.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-key-parsing/src/spki.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.120525 cryptography-42.0.6/src/rust/cryptography-openssl/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-openssl/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-openssl/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.120525 cryptography-42.0.6/src/rust/cryptography-openssl/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-openssl/src/aead.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-openssl/src/cmac.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-openssl/src/fips.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-openssl/src/hmac.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-openssl/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-openssl/src/poly1305.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.120525 cryptography-42.0.6/src/rust/cryptography-x509/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.124525 cryptography-42.0.6/src/rust/cryptography-x509/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    15429 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/common.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/crl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/csr.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/extensions.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/name.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/ocsp_req.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/ocsp_resp.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/oid.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509/src/pkcs7.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.120525 cryptography-42.0.6/src/rust/cryptography-x509-verification/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509-verification/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.120525 cryptography-42.0.6/src/rust/cryptography-x509-verification/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509-verification/src/certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509-verification/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509-verification/src/ops.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.120525 cryptography-42.0.6/src/rust/cryptography-x509-verification/src/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)    27310 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509-verification/src/policy/extension.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    31630 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509-verification/src/policy/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509-verification/src/trust_store.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    23407 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/cryptography-x509-verification/src/types.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.124525 cryptography-42.0.6/src/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/asn1.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.128525 cryptography-42.0.6/src/rust/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)    27626 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/aead.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/cipher_registry.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/cmac.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/dh.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    15169 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/dsa.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    22457 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/ec.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/ed25519.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/ed448.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/hashes.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/hmac.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/kdf.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/keys.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/poly1305.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    27628 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/rsa.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    16533 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/x25519.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/backend/x448.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/buf.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/exceptions.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/oid.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/padding.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    18084 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/pkcs7.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    21412 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/types.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.132525 cryptography-42.0.6/src/rust/src/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)    34292 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/common.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    24558 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/crl.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/csr.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    20006 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/extensions.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/ocsp.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/ocsp_req.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    30197 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/ocsp_resp.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/sct.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    25833 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/sign.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-04 15:22:57.000000 cryptography-42.0.6/src/rust/src/x509/verify.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.132525 cryptography-42.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.132525 cryptography-42.0.6/tests/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/bench/test_aead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/bench/test_ec_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/bench/test_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/bench/test_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/bench/test_x509.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/deprecated_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/doubles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.132525 cryptography-42.0.6/tests/hazmat/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.136525 cryptography-42.0.6/tests/hazmat/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/backends/test_openssl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.136525 cryptography-42.0.6/tests/hazmat/bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/bindings/test_openssl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.144526 cryptography-42.0.6/tests/hazmat/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/fixtures_dh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/fixtures_dsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/fixtures_ec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29306 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/fixtures_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_3des.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34423 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_aead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_aes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_aes_gcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_arc4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_asym_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_camellia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_cast5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_ciphers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6584 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_cmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9387 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_concatkdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_constant_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36388 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_dh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39026 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_dsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50088 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11313 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_ed448.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_hash_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_hkdf_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_hmac_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_idea.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26335 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_kbkdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_kbkdf_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_keywrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7877 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_pbkdf2hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34291 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_pkcs12.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35254 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_poly1305.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100702 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55602 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71151 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_x25519.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_x448.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_x963_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/test_x963kdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.144526 cryptography-42.0.6/tests/hazmat/primitives/twofactor/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/twofactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/twofactor/test_hotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/twofactor/test_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17277 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/hazmat/test_oid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/test_cryptography_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/test_fernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)   188472 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/test_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29808 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.148526 cryptography-42.0.6/tests/wycheproof/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_aes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_chacha20poly1305.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_cmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_dsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_ecdh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_eddsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_keywrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9962 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_x25519.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/test_x448.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/wycheproof/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.152526 cryptography-42.0.6/tests/x509/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/x509/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/x509/test_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55544 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/x509/test_ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   252838 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/x509/test_x509.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35375 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/x509/test_x509_crlbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)   218761 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/x509/test_x509_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7567 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/x509/test_x509_revokedcertbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 15:23:05.152526 cryptography-42.0.6/tests/x509/verification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/x509/verification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/x509/verification/test_limbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-04 15:22:57.000000 cryptography-42.0.6/tests/x509/verification/test_verification.py
```

### Comparing `cryptography-42.0.5/CHANGELOG.rst` & `cryptography-42.0.6/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+.. _v42-0-6:
+
+42.0.6 - 2024-05-04
+~~~~~~~~~~~~~~~~~~~
+
+* Fixed compilation when using LibreSSL 3.9.1.
+
 .. _v42-0-5:
 
 42.0.5 - 2024-02-23
 ~~~~~~~~~~~~~~~~~~~
 
 * Limit the number of name constraint checks that will be performed in
   :mod:`X.509 path validation <cryptography.x509.verification>` to protect
```

### Comparing `cryptography-42.0.5/CONTRIBUTING.rst` & `cryptography-42.0.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/LICENSE.APACHE` & `cryptography-42.0.6/LICENSE.APACHE`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/LICENSE.BSD` & `cryptography-42.0.6/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/MANIFEST.in` & `cryptography-42.0.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/PKG-INFO` & `cryptography-42.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptography
-Version: 42.0.5
+Version: 42.0.6
 Summary: cryptography is a package which provides cryptographic recipes and primitives to Python developers.
 Author-email: The Python Cryptographic Authority and individual contributors <cryptography-dev@python.org>
 License: Apache-2.0 OR BSD-3-Clause
 Project-URL: homepage, https://github.com/pyca/cryptography
 Project-URL: documentation, https://cryptography.io/
 Project-URL: source, https://github.com/pyca/cryptography/
 Project-URL: issues, https://github.com/pyca/cryptography/issues
```

### Comparing `cryptography-42.0.5/README.rst` & `cryptography-42.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/Makefile` & `cryptography-42.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/_ext/cryptography-docs.py` & `cryptography-42.0.6/docs/_ext/cryptography-docs.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/_ext/linkcode_res.py` & `cryptography-42.0.6/docs/_ext/linkcode_res.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/api-stability.rst` & `cryptography-42.0.6/docs/api-stability.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/community.rst` & `cryptography-42.0.6/docs/community.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/conf.py` & `cryptography-42.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/c-bindings.rst` & `cryptography-42.0.6/docs/development/c-bindings.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/aes-192-gcm-siv/generate_aes192gcmsiv.py` & `cryptography-42.0.6/docs/development/custom-vectors/aes-192-gcm-siv/generate_aes192gcmsiv.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/aes-192-gcm-siv/verify-aes192gcmsiv/src/main.rs` & `cryptography-42.0.6/docs/development/custom-vectors/aes-192-gcm-siv/verify-aes192gcmsiv/src/main.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/aes-192-gcm-siv.rst` & `cryptography-42.0.6/docs/development/custom-vectors/aes-192-gcm-siv.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/arc4/generate_arc4.py` & `cryptography-42.0.6/docs/development/custom-vectors/arc4/generate_arc4.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/arc4/verify_arc4.go` & `cryptography-42.0.6/docs/development/custom-vectors/arc4/verify_arc4.go`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/arc4.rst` & `cryptography-42.0.6/docs/development/custom-vectors/arc4.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/cast5/generate_cast5.py` & `cryptography-42.0.6/docs/development/custom-vectors/cast5/generate_cast5.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/cast5/verify_cast5.go` & `cryptography-42.0.6/docs/development/custom-vectors/cast5/verify_cast5.go`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/cast5.rst` & `cryptography-42.0.6/docs/development/custom-vectors/cast5.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/chacha20/generate_chacha20_overflow.py` & `cryptography-42.0.6/docs/development/custom-vectors/chacha20/generate_chacha20_overflow.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/chacha20/verify_chacha20_overflow.py` & `cryptography-42.0.6/docs/development/custom-vectors/chacha20/verify_chacha20_overflow.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/chacha20.rst` & `cryptography-42.0.6/docs/development/custom-vectors/chacha20.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/hkdf/generate_hkdf.py` & `cryptography-42.0.6/docs/development/custom-vectors/hkdf/generate_hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/hkdf/verify_hkdf.go` & `cryptography-42.0.6/docs/development/custom-vectors/hkdf/verify_hkdf.go`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/hkdf.rst` & `cryptography-42.0.6/docs/development/custom-vectors/hkdf.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/idea/generate_idea.py` & `cryptography-42.0.6/docs/development/custom-vectors/idea/generate_idea.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/idea/verify_idea.py` & `cryptography-42.0.6/docs/development/custom-vectors/idea/verify_idea.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/idea.rst` & `cryptography-42.0.6/docs/development/custom-vectors/idea.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java` & `cryptography-42.0.6/docs/development/custom-vectors/rsa-oaep-sha2/VerifyRSAOAEPSHA2.java`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py` & `cryptography-42.0.6/docs/development/custom-vectors/rsa-oaep-sha2/generate_rsa_oaep_sha2.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/rsa-oaep-sha2.rst` & `cryptography-42.0.6/docs/development/custom-vectors/rsa-oaep-sha2.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/secp256k1/generate_secp256k1.py` & `cryptography-42.0.6/docs/development/custom-vectors/secp256k1/generate_secp256k1.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/secp256k1/verify_secp256k1.py` & `cryptography-42.0.6/docs/development/custom-vectors/secp256k1/verify_secp256k1.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/secp256k1.rst` & `cryptography-42.0.6/docs/development/custom-vectors/secp256k1.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/seed/generate_seed.py` & `cryptography-42.0.6/docs/development/custom-vectors/seed/generate_seed.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/seed/verify_seed.py` & `cryptography-42.0.6/docs/development/custom-vectors/seed/verify_seed.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/custom-vectors/seed.rst` & `cryptography-42.0.6/docs/development/custom-vectors/seed.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/getting-started.rst` & `cryptography-42.0.6/docs/development/getting-started.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/index.rst` & `cryptography-42.0.6/docs/development/index.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/reviewing-patches.rst` & `cryptography-42.0.6/docs/development/reviewing-patches.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/submitting-patches.rst` & `cryptography-42.0.6/docs/development/submitting-patches.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/development/test-vectors.rst` & `cryptography-42.0.6/docs/development/test-vectors.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/doing-a-release.rst` & `cryptography-42.0.6/docs/doing-a-release.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/exceptions.rst` & `cryptography-42.0.6/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/faq.rst` & `cryptography-42.0.6/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/fernet.rst` & `cryptography-42.0.6/docs/fernet.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/glossary.rst` & `cryptography-42.0.6/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/aead.rst` & `cryptography-42.0.6/docs/hazmat/primitives/aead.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/dh.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/dh.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/dsa.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/dsa.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/ec.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/ec.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/ed25519.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/ed25519.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/ed448.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/ed448.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/index.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/index.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/rsa.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/rsa.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/serialization.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/serialization.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/utils.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/utils.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/x25519.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/x25519.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/asymmetric/x448.rst` & `cryptography-42.0.6/docs/hazmat/primitives/asymmetric/x448.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/constant-time.rst` & `cryptography-42.0.6/docs/hazmat/primitives/constant-time.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/cryptographic-hashes.rst` & `cryptography-42.0.6/docs/hazmat/primitives/cryptographic-hashes.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/key-derivation-functions.rst` & `cryptography-42.0.6/docs/hazmat/primitives/key-derivation-functions.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/keywrap.rst` & `cryptography-42.0.6/docs/hazmat/primitives/keywrap.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/mac/cmac.rst` & `cryptography-42.0.6/docs/hazmat/primitives/mac/cmac.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/mac/hmac.rst` & `cryptography-42.0.6/docs/hazmat/primitives/mac/hmac.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/mac/poly1305.rst` & `cryptography-42.0.6/docs/hazmat/primitives/mac/poly1305.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/padding.rst` & `cryptography-42.0.6/docs/hazmat/primitives/padding.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/symmetric-encryption.rst` & `cryptography-42.0.6/docs/hazmat/primitives/symmetric-encryption.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/hazmat/primitives/twofactor.rst` & `cryptography-42.0.6/docs/hazmat/primitives/twofactor.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/index.rst` & `cryptography-42.0.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/installation.rst` & `cryptography-42.0.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/limitations.rst` & `cryptography-42.0.6/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/make.bat` & `cryptography-42.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/openssl.rst` & `cryptography-42.0.6/docs/openssl.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/random-numbers.rst` & `cryptography-42.0.6/docs/random-numbers.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/security.rst` & `cryptography-42.0.6/docs/security.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/spelling_wordlist.txt` & `cryptography-42.0.6/docs/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/x509/certificate-transparency.rst` & `cryptography-42.0.6/docs/x509/certificate-transparency.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/x509/ocsp.rst` & `cryptography-42.0.6/docs/x509/ocsp.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/x509/reference.rst` & `cryptography-42.0.6/docs/x509/reference.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/x509/tutorial.rst` & `cryptography-42.0.6/docs/x509/tutorial.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/docs/x509/verification.rst` & `cryptography-42.0.6/docs/x509/verification.rst`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/noxfile.py` & `cryptography-42.0.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/pyproject.toml` & `cryptography-42.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "cffi>=1.12; platform_python_implementation != 'PyPy'",
     "setuptools-rust>=1.7.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cryptography"
-version = "42.0.5"
+version = "42.0.6"
 authors = [
     {name = "The Python Cryptographic Authority and individual contributors", email = "cryptography-dev@python.org"}
 ]
 description = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
 readme = "README.rst"
 license = {text = "Apache-2.0 OR BSD-3-Clause"}
 classifiers = [
```

### Comparing `cryptography-42.0.5/src/_cffi_src/build_openssl.py` & `cryptography-42.0.6/src/_cffi_src/build_openssl.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/asn1.py` & `cryptography-42.0.6/src/_cffi_src/openssl/asn1.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/bignum.py` & `cryptography-42.0.6/src/_cffi_src/openssl/bignum.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/bio.py` & `cryptography-42.0.6/src/_cffi_src/openssl/bio.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/crypto.py` & `cryptography-42.0.6/src/_cffi_src/openssl/crypto.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/cryptography.py` & `cryptography-42.0.6/src/_cffi_src/openssl/cryptography.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/dsa.py` & `cryptography-42.0.6/src/_cffi_src/openssl/dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/ec.py` & `cryptography-42.0.6/src/_cffi_src/openssl/ec.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/engine.py` & `cryptography-42.0.6/src/_cffi_src/openssl/engine.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/err.py` & `cryptography-42.0.6/src/_cffi_src/openssl/err.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/evp.py` & `cryptography-42.0.6/src/_cffi_src/openssl/evp.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/nid.py` & `cryptography-42.0.6/src/_cffi_src/openssl/nid.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/opensslv.py` & `cryptography-42.0.6/src/_cffi_src/openssl/opensslv.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/pem.py` & `cryptography-42.0.6/src/_cffi_src/openssl/pem.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/pkcs12.py` & `cryptography-42.0.6/src/_cffi_src/openssl/pkcs12.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/pkcs7.py` & `cryptography-42.0.6/src/_cffi_src/openssl/pkcs7.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/provider.py` & `cryptography-42.0.6/src/_cffi_src/openssl/provider.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/rsa.py` & `cryptography-42.0.6/src/_cffi_src/openssl/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/ssl.py` & `cryptography-42.0.6/src/_cffi_src/openssl/ssl.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/x509.py` & `cryptography-42.0.6/src/_cffi_src/openssl/x509.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/x509_vfy.py` & `cryptography-42.0.6/src/_cffi_src/openssl/x509_vfy.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/x509name.py` & `cryptography-42.0.6/src/_cffi_src/openssl/x509name.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/openssl/x509v3.py` & `cryptography-42.0.6/src/_cffi_src/openssl/x509v3.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/_cffi_src/utils.py` & `cryptography-42.0.6/src/_cffi_src/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/exceptions.py` & `cryptography-42.0.6/src/cryptography/exceptions.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/fernet.py` & `cryptography-42.0.6/src/cryptography/fernet.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/_oid.py` & `cryptography-42.0.6/src/cryptography/hazmat/_oid.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/backends/openssl/aead.py` & `cryptography-42.0.6/src/cryptography/hazmat/backends/openssl/aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/backends/openssl/backend.py` & `cryptography-42.0.6/src/cryptography/hazmat/backends/openssl/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,28 +531,20 @@
     def dh_supported(self) -> bool:
         return not self._lib.CRYPTOGRAPHY_IS_BORINGSSL
 
     def dh_x942_serialization_supported(self) -> bool:
         return self._lib.Cryptography_HAS_EVP_PKEY_DHX == 1
 
     def x25519_supported(self) -> bool:
-        # Beginning with OpenSSL 3.2.0, X25519 is considered FIPS.
-        if (
-            self._fips_enabled
-            and not self._lib.CRYPTOGRAPHY_OPENSSL_320_OR_GREATER
-        ):
+        if self._fips_enabled:
             return False
         return True
 
     def x448_supported(self) -> bool:
-        # Beginning with OpenSSL 3.2.0, X448 is considered FIPS.
-        if (
-            self._fips_enabled
-            and not self._lib.CRYPTOGRAPHY_OPENSSL_320_OR_GREATER
-        ):
+        if self._fips_enabled:
             return False
         return (
             not self._lib.CRYPTOGRAPHY_IS_LIBRESSL
             and not self._lib.CRYPTOGRAPHY_IS_BORINGSSL
         )
 
     def ed25519_supported(self) -> bool:
```

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/backends/openssl/ciphers.py` & `cryptography-42.0.6/src/cryptography/hazmat/backends/openssl/ciphers.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/backends/openssl/decode_asn1.py` & `cryptography-42.0.6/src/cryptography/hazmat/backends/openssl/decode_asn1.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/asn1.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/asn1.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/exceptions.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/ocsp.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/ocsp.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/aead.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/aead.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/cmac.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/cmac.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/dh.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/dh.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/ec.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/ec.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/keys.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/keys.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/openssl/rsa.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/openssl/rsa.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/pkcs7.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/pkcs7.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/_rust/x509.pyi` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/_rust/x509.pyi`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/openssl/_conditional.py` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/openssl/_conditional.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/bindings/openssl/binding.py` & `cryptography-42.0.6/src/cryptography/hazmat/bindings/openssl/binding.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/_asymmetric.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/_asymmetric.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/_cipheralgorithm.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/_cipheralgorithm.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/_serialization.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/_serialization.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/dh.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/dh.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/dsa.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/ec.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/ec.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/ed25519.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/ed25519.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/ed448.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/ed448.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/padding.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/padding.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/rsa.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/types.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/types.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/utils.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/x25519.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/x25519.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/asymmetric/x448.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/asymmetric/x448.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/__init__.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/aead.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/algorithms.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/algorithms.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/base.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/base.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/ciphers/modes.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/ciphers/modes.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/hashes.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/hashes.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/__init__.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/concatkdf.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/concatkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/hkdf.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/kbkdf.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/kbkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/pbkdf2.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/scrypt.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/scrypt.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/kdf/x963kdf.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/kdf/x963kdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/keywrap.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/keywrap.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/padding.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/padding.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/__init__.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/base.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/base.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/pkcs12.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/pkcs12.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/pkcs7.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/pkcs7.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/serialization/ssh.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/serialization/ssh.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/twofactor/hotp.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/twofactor/hotp.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/hazmat/primitives/twofactor/totp.py` & `cryptography-42.0.6/src/cryptography/hazmat/primitives/twofactor/totp.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/utils.py` & `cryptography-42.0.6/src/cryptography/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/x509/__init__.py` & `cryptography-42.0.6/src/cryptography/x509/__init__.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/x509/base.py` & `cryptography-42.0.6/src/cryptography/x509/base.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/x509/certificate_transparency.py` & `cryptography-42.0.6/src/cryptography/x509/certificate_transparency.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/x509/extensions.py` & `cryptography-42.0.6/src/cryptography/x509/extensions.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/x509/general_name.py` & `cryptography-42.0.6/src/cryptography/x509/general_name.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/x509/name.py` & `cryptography-42.0.6/src/cryptography/x509/name.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/x509/ocsp.py` & `cryptography-42.0.6/src/cryptography/x509/ocsp.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/x509/oid.py` & `cryptography-42.0.6/src/cryptography/x509/oid.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography/x509/verification.py` & `cryptography-42.0.6/src/cryptography/x509/verification.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/cryptography.egg-info/PKG-INFO` & `cryptography-42.0.6/src/cryptography.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptography
-Version: 42.0.5
+Version: 42.0.6
 Summary: cryptography is a package which provides cryptographic recipes and primitives to Python developers.
 Author-email: The Python Cryptographic Authority and individual contributors <cryptography-dev@python.org>
 License: Apache-2.0 OR BSD-3-Clause
 Project-URL: homepage, https://github.com/pyca/cryptography
 Project-URL: documentation, https://cryptography.io/
 Project-URL: source, https://github.com/pyca/cryptography/
 Project-URL: issues, https://github.com/pyca/cryptography/issues
```

### Comparing `cryptography-42.0.5/src/cryptography.egg-info/SOURCES.txt` & `cryptography-42.0.6/src/cryptography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/Cargo.lock` & `cryptography-42.0.6/src/rust/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -185,17 +185,17 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "openssl"
-version = "0.10.63"
+version = "0.10.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15c9d69dd87a29568d4d017cfe8ec518706046a05184e5aea92d0af890b803c8"
+checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
 dependencies = [
  "bitflags 2.4.2",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -211,17 +211,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.99"
+version = "0.9.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22e1bf214306098e4832460f797824c05d25aacdf896f64a985fb0fd992454ae"
+checksum = "c597637d56fbc83893a35eb0dd04b2b8e7a50c91e64e9493e398b5df4fb45fa2"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
```

### Comparing `cryptography-42.0.5/src/rust/Cargo.toml` & `cryptography-42.0.6/src/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/build.rs` & `cryptography-42.0.6/src/rust/build.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-cffi/build.rs` & `cryptography-42.0.6/src/rust/cryptography-cffi/build.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-cffi/src/lib.rs` & `cryptography-42.0.6/src/rust/cryptography-cffi/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -23,12 +23,12 @@
         assert_eq!(res, 0);
         pyo3::types::PyModule::import(py, "_openssl")?
     };
     #[cfg(not(python_implementation = "PyPy"))]
     // SAFETY: `PyInit__openssl` returns an owned reference.
     let openssl_mod = unsafe {
         let ptr = PyInit__openssl();
-        pyo3::types::PyModule::from_owned_ptr(py, ptr)
+        pyo3::types::PyModule::from_owned_ptr_or_err(py, ptr)?
     };
 
     Ok(openssl_mod)
 }
```

### Comparing `cryptography-42.0.5/src/rust/cryptography-key-parsing/src/lib.rs` & `cryptography-42.0.6/src/rust/cryptography-key-parsing/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-key-parsing/src/rsa.rs` & `cryptography-42.0.6/src/rust/cryptography-key-parsing/src/rsa.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-key-parsing/src/spki.rs` & `cryptography-42.0.6/src/rust/cryptography-key-parsing/src/spki.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-openssl/build.rs` & `cryptography-42.0.6/src/rust/cryptography-openssl/build.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-openssl/src/aead.rs` & `cryptography-42.0.6/src/rust/cryptography-openssl/src/aead.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-openssl/src/cmac.rs` & `cryptography-42.0.6/src/rust/cryptography-openssl/src/cmac.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-openssl/src/fips.rs` & `cryptography-42.0.6/src/rust/cryptography-openssl/src/fips.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-openssl/src/hmac.rs` & `cryptography-42.0.6/src/rust/cryptography-openssl/src/hmac.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-openssl/src/lib.rs` & `cryptography-42.0.6/src/rust/cryptography-openssl/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-openssl/src/poly1305.rs` & `cryptography-42.0.6/src/rust/cryptography-openssl/src/poly1305.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509/src/certificate.rs` & `cryptography-42.0.6/src/rust/cryptography-x509/src/certificate.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509/src/common.rs` & `cryptography-42.0.6/src/rust/cryptography-x509/src/common.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509/src/crl.rs` & `cryptography-42.0.6/src/rust/cryptography-x509/src/crl.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509/src/csr.rs` & `cryptography-42.0.6/src/rust/cryptography-x509/src/csr.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509/src/extensions.rs` & `cryptography-42.0.6/src/rust/cryptography-x509/src/extensions.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509/src/name.rs` & `cryptography-42.0.6/src/rust/cryptography-x509/src/name.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509/src/ocsp_req.rs` & `cryptography-42.0.6/src/rust/cryptography-x509/src/ocsp_req.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509/src/ocsp_resp.rs` & `cryptography-42.0.6/src/rust/cryptography-x509/src/ocsp_resp.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509/src/oid.rs` & `cryptography-42.0.6/src/rust/cryptography-x509/src/oid.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509/src/pkcs7.rs` & `cryptography-42.0.6/src/rust/cryptography-x509/src/pkcs7.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509-verification/src/certificate.rs` & `cryptography-42.0.6/src/rust/cryptography-x509-verification/src/certificate.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509-verification/src/lib.rs` & `cryptography-42.0.6/src/rust/cryptography-x509-verification/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509-verification/src/ops.rs` & `cryptography-42.0.6/src/rust/cryptography-x509-verification/src/ops.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509-verification/src/policy/extension.rs` & `cryptography-42.0.6/src/rust/cryptography-x509-verification/src/policy/extension.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509-verification/src/policy/mod.rs` & `cryptography-42.0.6/src/rust/cryptography-x509-verification/src/policy/mod.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509-verification/src/trust_store.rs` & `cryptography-42.0.6/src/rust/cryptography-x509-verification/src/trust_store.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/cryptography-x509-verification/src/types.rs` & `cryptography-42.0.6/src/rust/cryptography-x509-verification/src/types.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/asn1.rs` & `cryptography-42.0.6/src/rust/src/asn1.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/aead.rs` & `cryptography-42.0.6/src/rust/src/backend/aead.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/cipher_registry.rs` & `cryptography-42.0.6/src/rust/src/backend/cipher_registry.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/cmac.rs` & `cryptography-42.0.6/src/rust/src/backend/cmac.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/dh.rs` & `cryptography-42.0.6/src/rust/src/backend/dh.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/dsa.rs` & `cryptography-42.0.6/src/rust/src/backend/dsa.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/ec.rs` & `cryptography-42.0.6/src/rust/src/backend/ec.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/ed25519.rs` & `cryptography-42.0.6/src/rust/src/backend/ed25519.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/ed448.rs` & `cryptography-42.0.6/src/rust/src/backend/ed448.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/hashes.rs` & `cryptography-42.0.6/src/rust/src/backend/hashes.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/hmac.rs` & `cryptography-42.0.6/src/rust/src/backend/hmac.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/kdf.rs` & `cryptography-42.0.6/src/rust/src/backend/kdf.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/keys.rs` & `cryptography-42.0.6/src/rust/src/backend/keys.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/mod.rs` & `cryptography-42.0.6/src/rust/src/backend/mod.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/poly1305.rs` & `cryptography-42.0.6/src/rust/src/backend/poly1305.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/rsa.rs` & `cryptography-42.0.6/src/rust/src/backend/rsa.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/utils.rs` & `cryptography-42.0.6/src/rust/src/backend/utils.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/x25519.rs` & `cryptography-42.0.6/src/rust/src/backend/x25519.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/backend/x448.rs` & `cryptography-42.0.6/src/rust/src/backend/x448.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/buf.rs` & `cryptography-42.0.6/src/rust/src/buf.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/error.rs` & `cryptography-42.0.6/src/rust/src/error.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/exceptions.rs` & `cryptography-42.0.6/src/rust/src/exceptions.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/lib.rs` & `cryptography-42.0.6/src/rust/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 // This file is dual licensed under the terms of the Apache License, Version
 // 2.0, and the BSD License. See the LICENSE file in the root of this repository
 // for complete details.
 
 #![deny(rust_2018_idioms, clippy::undocumented_unsafe_blocks)]
+#![allow(unknown_lints, non_local_definitions)]
 
 use crate::error::CryptographyResult;
 #[cfg(CRYPTOGRAPHY_OPENSSL_300_OR_GREATER)]
 use openssl::provider;
 use std::env;
 
 mod asn1;
```

### Comparing `cryptography-42.0.5/src/rust/src/oid.rs` & `cryptography-42.0.6/src/rust/src/oid.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/padding.rs` & `cryptography-42.0.6/src/rust/src/padding.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/pkcs7.rs` & `cryptography-42.0.6/src/rust/src/pkcs7.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/types.rs` & `cryptography-42.0.6/src/rust/src/types.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/x509/certificate.rs` & `cryptography-42.0.6/src/rust/src/x509/certificate.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/x509/common.rs` & `cryptography-42.0.6/src/rust/src/x509/common.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/x509/crl.rs` & `cryptography-42.0.6/src/rust/src/x509/crl.rs`

 * *Files 1% similar despite different names*

```diff
@@ -451,19 +451,26 @@
     it: &mut OwnedCRLIteratorData,
     f: impl for<'this> FnOnce(
         &'this OwnedCertificateRevocationList,
         &mut Option<asn1::SequenceOf<'this, crl::RevokedCertificate<'this>>>,
     ) -> Result<crl::RevokedCertificate<'this>, E>,
 ) -> Result<OwnedRevokedCertificate, E> {
     OwnedRevokedCertificate::try_new(Arc::clone(it.borrow_owner()), |inner_it| {
-        // SAFETY: This is safe because `Arc::clone` ensures the data is
-        // alive, but Rust doesn't understand the lifetime relationship it
-        // produces. Open-coded implementation of the API discussed in
-        // https://github.com/joshua-maros/ouroboros/issues/38
-        it.with_dependent_mut(|_, value| f(inner_it, unsafe { std::mem::transmute(value) }))
+        it.with_dependent_mut(|_, value| {
+            // SAFETY: This is safe because `Arc::clone` ensures the data is
+            // alive, but Rust doesn't understand the lifetime relationship it
+            // produces. Open-coded implementation of the API discussed in
+            // https://github.com/joshua-maros/ouroboros/issues/38
+            f(inner_it, unsafe {
+                std::mem::transmute::<
+                    &mut Option<asn1::SequenceOf<'_, crl::RevokedCertificate<'_>>>,
+                    &mut Option<asn1::SequenceOf<'_, crl::RevokedCertificate<'_>>>,
+                >(value)
+            })
+        })
     })
 }
 
 #[pyo3::prelude::pymethods]
 impl CRLIterator {
     fn __len__(&self) -> usize {
         self.contents
```

### Comparing `cryptography-42.0.5/src/rust/src/x509/csr.rs` & `cryptography-42.0.6/src/rust/src/x509/csr.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/x509/extensions.rs` & `cryptography-42.0.6/src/rust/src/x509/extensions.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/x509/mod.rs` & `cryptography-42.0.6/src/rust/src/x509/mod.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/x509/ocsp.rs` & `cryptography-42.0.6/src/rust/src/x509/ocsp.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/x509/ocsp_req.rs` & `cryptography-42.0.6/src/rust/src/x509/ocsp_req.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/x509/ocsp_resp.rs` & `cryptography-42.0.6/src/rust/src/x509/ocsp_resp.rs`

 * *Files 0% similar despite different names*

```diff
@@ -414,31 +414,42 @@
 ) -> certificate::OwnedCertificate {
     certificate::OwnedCertificate::new(it.borrow_owner().clone_ref(py), |inner_it| {
         it.with_dependent(|_, value| {
             // SAFETY: This is safe because `Arc::clone` ensures the data is
             // alive, but Rust doesn't understand the lifetime relationship it
             // produces. Open-coded implementation of the API discussed in
             // https://github.com/joshua-maros/ouroboros/issues/38
-            f(inner_it.as_bytes(py), unsafe { std::mem::transmute(value) })
+            f(inner_it.as_bytes(py), unsafe {
+                std::mem::transmute::<&ocsp_resp::OCSPResponse<'_>, &ocsp_resp::OCSPResponse<'_>>(
+                    value,
+                )
+            })
         })
     })
 }
 fn try_map_arc_data_mut_ocsp_response_iterator<E>(
     it: &mut OwnedOCSPResponseIteratorData,
     f: impl for<'this> FnOnce(
         &'this OwnedOCSPResponse,
         &mut asn1::SequenceOf<'this, ocsp_resp::SingleResponse<'this>>,
     ) -> Result<ocsp_resp::SingleResponse<'this>, E>,
 ) -> Result<OwnedSingleResponse, E> {
     OwnedSingleResponse::try_new(Arc::clone(it.borrow_owner()), |inner_it| {
-        // SAFETY: This is safe because `Arc::clone` ensures the data is
-        // alive, but Rust doesn't understand the lifetime relationship it
-        // produces. Open-coded implementation of the API discussed in
-        // https://github.com/joshua-maros/ouroboros/issues/38
-        it.with_dependent_mut(|_, value| f(inner_it, unsafe { std::mem::transmute(value) }))
+        it.with_dependent_mut(|_, value| {
+            // SAFETY: This is safe because `Arc::clone` ensures the data is
+            // alive, but Rust doesn't understand the lifetime relationship it
+            // produces. Open-coded implementation of the API discussed in
+            // https://github.com/joshua-maros/ouroboros/issues/38
+            f(inner_it, unsafe {
+                std::mem::transmute::<
+                    &mut asn1::SequenceOf<'_, ocsp_resp::SingleResponse<'_>>,
+                    &mut asn1::SequenceOf<'_, ocsp_resp::SingleResponse<'_>>,
+                >(value)
+            })
+        })
     })
 }
 
 fn single_response<'a>(
     resp: &ocsp_resp::BasicOCSPResponse<'a>,
 ) -> Result<ocsp_resp::SingleResponse<'a>, CryptographyError> {
     let responses = resp.tbs_response_data.responses.unwrap_read();
```

### Comparing `cryptography-42.0.5/src/rust/src/x509/sct.rs` & `cryptography-42.0.6/src/rust/src/x509/sct.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/x509/sign.rs` & `cryptography-42.0.6/src/rust/src/x509/sign.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/src/rust/src/x509/verify.rs` & `cryptography-42.0.6/src/rust/src/x509/verify.rs`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/bench/test_aead.py` & `cryptography-42.0.6/tests/bench/test_aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/bench/test_x509.py` & `cryptography-42.0.6/tests/bench/test_x509.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/conftest.py` & `cryptography-42.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/doubles.py` & `cryptography-42.0.6/tests/doubles.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/backends/test_openssl.py` & `cryptography-42.0.6/tests/hazmat/backends/test_openssl.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/bindings/test_openssl.py` & `cryptography-42.0.6/tests/hazmat/bindings/test_openssl.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/fixtures_dh.py` & `cryptography-42.0.6/tests/hazmat/primitives/fixtures_dh.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/fixtures_dsa.py` & `cryptography-42.0.6/tests/hazmat/primitives/fixtures_dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/fixtures_ec.py` & `cryptography-42.0.6/tests/hazmat/primitives/fixtures_ec.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/fixtures_rsa.py` & `cryptography-42.0.6/tests/hazmat/primitives/fixtures_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_3des.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_3des.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_aead.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_aead.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_aes.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_aes.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_aes_gcm.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_aes_gcm.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_arc4.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_arc4.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_asym_utils.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_asym_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_block.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_block.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_blowfish.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_blowfish.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_camellia.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_camellia.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_cast5.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_cast5.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_chacha20.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_chacha20.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_ciphers.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_ciphers.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_cmac.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_cmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_concatkdf.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_concatkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_constant_time.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_constant_time.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_dh.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_dh.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_dsa.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_ec.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_ec.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_ed25519.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_ed25519.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_ed448.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_ed448.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_hash_vectors.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_hash_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_hashes.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_hashes.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_hkdf.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_hkdf_vectors.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_hkdf_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_hmac.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_hmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_hmac_vectors.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_hmac_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_idea.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_idea.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_kbkdf.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_kbkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_keywrap.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_keywrap.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_padding.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_padding.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_pbkdf2hmac.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_pbkdf2hmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_pbkdf2hmac_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_pkcs12.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_pkcs12.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_pkcs7.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_pkcs7.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_poly1305.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_poly1305.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_rsa.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_scrypt.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_scrypt.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_seed.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_seed.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_serialization.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_serialization.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_sm4.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_sm4.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_ssh.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_ssh.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_x25519.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_x25519.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_x448.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_x448.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_x963_vectors.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_x963_vectors.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/test_x963kdf.py` & `cryptography-42.0.6/tests/hazmat/primitives/test_x963kdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/twofactor/test_hotp.py` & `cryptography-42.0.6/tests/hazmat/primitives/twofactor/test_hotp.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/twofactor/test_totp.py` & `cryptography-42.0.6/tests/hazmat/primitives/twofactor/test_totp.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/primitives/utils.py` & `cryptography-42.0.6/tests/hazmat/primitives/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/hazmat/test_oid.py` & `cryptography-42.0.6/tests/hazmat/test_oid.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/test_cryptography_utils.py` & `cryptography-42.0.6/tests/test_cryptography_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/test_fernet.py` & `cryptography-42.0.6/tests/test_fernet.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/test_meta.py` & `cryptography-42.0.6/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/test_utils.py` & `cryptography-42.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/test_warnings.py` & `cryptography-42.0.6/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/utils.py` & `cryptography-42.0.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_aes.py` & `cryptography-42.0.6/tests/wycheproof/test_aes.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_chacha20poly1305.py` & `cryptography-42.0.6/tests/wycheproof/test_chacha20poly1305.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_cmac.py` & `cryptography-42.0.6/tests/wycheproof/test_cmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_dsa.py` & `cryptography-42.0.6/tests/wycheproof/test_dsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_ecdh.py` & `cryptography-42.0.6/tests/wycheproof/test_ecdh.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_ecdsa.py` & `cryptography-42.0.6/tests/wycheproof/test_ecdsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_eddsa.py` & `cryptography-42.0.6/tests/wycheproof/test_eddsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_hkdf.py` & `cryptography-42.0.6/tests/wycheproof/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_hmac.py` & `cryptography-42.0.6/tests/wycheproof/test_hmac.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_keywrap.py` & `cryptography-42.0.6/tests/wycheproof/test_keywrap.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_pbkdf2.py` & `cryptography-42.0.6/tests/wycheproof/test_pbkdf2.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_rsa.py` & `cryptography-42.0.6/tests/wycheproof/test_rsa.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_x25519.py` & `cryptography-42.0.6/tests/wycheproof/test_x25519.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/test_x448.py` & `cryptography-42.0.6/tests/wycheproof/test_x448.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/wycheproof/utils.py` & `cryptography-42.0.6/tests/wycheproof/utils.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/x509/test_name.py` & `cryptography-42.0.6/tests/x509/test_name.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/x509/test_ocsp.py` & `cryptography-42.0.6/tests/x509/test_ocsp.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/x509/test_x509.py` & `cryptography-42.0.6/tests/x509/test_x509.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/x509/test_x509_crlbuilder.py` & `cryptography-42.0.6/tests/x509/test_x509_crlbuilder.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/x509/test_x509_ext.py` & `cryptography-42.0.6/tests/x509/test_x509_ext.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/x509/test_x509_revokedcertbuilder.py` & `cryptography-42.0.6/tests/x509/test_x509_revokedcertbuilder.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/x509/verification/test_limbo.py` & `cryptography-42.0.6/tests/x509/verification/test_limbo.py`

 * *Files identical despite different names*

### Comparing `cryptography-42.0.5/tests/x509/verification/test_verification.py` & `cryptography-42.0.6/tests/x509/verification/test_verification.py`

 * *Files identical despite different names*

