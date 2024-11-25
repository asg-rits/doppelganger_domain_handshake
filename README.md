# List of Doppelganger domains registered to Handshake distributed naming service

## Preface
We identified in our paper that many doppelgdanger domains are registered to the Handshake
distributed naming service. This repository provides the list of such domains we extracted from the Handshake transactions.

## What is covered and what is not covered
We define a top level domain (TLD) registered to Handshake as a _doppelgdanger domain_ of  _a legitimate domain_ if the TLD in Handshake is a suffix of a string given by excluding the dots (.) from the legitimate domain. Here, a legitimate domain is a domain of any level that can be reached from ICANN TLDs. Suffixes of a string include the string itself (i.e., "str" is a suffix of "str").

The below table shows examples of legitimate domains and possible doppelganger domains for each of them.

| Legitimate Domain | Doppelgdanger Domain(s) |
----|---- 
| .com | .om |
| .google.com | .glecom, .googlecom |

The blow are examples of domains **not** regarded as doppelgdanger domains under our definition.

| Legitimate Domain | Non-Doppelgdanger Domain |
----|---- 
| .com | .coom |
| .google.com | .googlecomfakedomain |

## The List
We provide the list of doppelganger domains registered to Handshake that corresponds to top-N popular domains 
in the [Cloudflare's domain ranking](https://radar.cloudflare.com/domains).

- [List for top-100 popular domains](/doppelganger_domain_handshake_top_100.csv)
  - Ordered by the popularity of the legitimate domains
- [List for top-1000 popular domains](/doppelganger_domain_handshake_top_1000.csv)
  - Ordered alphabetically
  - The Cloudflare's list itself is not ordered by the popularity :thinking: 

Each line of a list contains a legitimate domain followed by doppelgdanger domains of that domain registered to Handshake.

```
legitimate domain 1, doppelgdanger domain 1, doppelgdanger domain 2, ...
...
```

## Citation
Please cite our paper when you use the lists we provide.

The citation should look like this in a paper written in English (or any non-Japanese language):

> Junichi Yoshida, Soramichi Akiyama: "Quantitative Analysis of Doppelgänger Domains Registered to Decentralized Naming Service Handshake (in Japanese)", Internet and Operation Technology Symposium (IOTS), pp. ? - ?, 2024.

The citation should look like this in a paper written in Japanese:

> 吉田純一, 穐山空道: "分散型ネーミングサービスHandshake に登録されたドッペルゲンガードメインの定量的調査", インターネットと運用技術シンポジウム (IOTS), pp. ? - ?, 2024.

## Contact
[Soramichi Akiyama](https://www.soramichi.jp) (College of Information Science and Engineering, Ritsumeikan University)
