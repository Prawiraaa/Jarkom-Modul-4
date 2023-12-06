| Name                              | NRP        |
|-----------------------------------|------------|
|I Putu Arya Prawira Wiwekananda    | 5025211065 |
|Hanifi Abrar Setiawan              | 5025211066 |
|Muhammad Fadhlan Ashila Harastha   | 5025211068 |

## Question

1. Gunakan prefix IP sesuai dengan prefix IP masing-masing.<br>
2. Terdapat template spreadsheet untuk mempermudah penilaian, gunakan template tersebut untuk melakukan penghitungan subnetting.<br>
3. Hasil perhitungan subnetting dan pohon pembagian IP serta file .pkt di submit pada link di atas.<br>
4. File yang didemokan adalah file .pkt yang telah disubmit.<br>
5. Pengurangan nilai akan dilakukan ketika:
- Melanggar salah satu dari tulisan diatas.
- Tidak menggunakan PREFIX ip yang ditetapkan sebelumnya
- Hasil perhitungan untuk VLSM / CIDR, berbeda dengan di CPT / GNS3
- Pembagian IP kurang efisien
- Routing kurang efisien
- Tidak bisa menjelaskan cara perhitungan VLSM dan CIDR

### Topologi GNS3 - VLSM
## Subnet Table for VLSM
| Subnet | Host IP | Netmask |
|--------|---------|---------|
| A1     | 1023    | /21     |
| A2     | 1001    | /22     |
| A3     | 6       | /29     |
| A4     | 512     | /22     |
| A5     | 31      | /26     |
| A6     | 2       | /30     |
| A7     | 3       | /29     |
| A8     | 2       | /30     |
| A9     | 2       | /30     |
| A10    | 25      | /27     |
| A11    | 2       | /30     |
| A12    | 2       | /30     |
| A13    | 255     | /23     |
| A14    | 2       | /30     |
| A15    | 2       | /30     |
| A16    | 2       | /30     |
| A17    | 2       | /30     |
| A18    | 127     | /25     |
| A19    | 1001    | /22     |
| A20    | 251     | /24     |
| A21    | 2       | /30     |

![Topology](https://cdn.discordapp.com/attachments/827014097219878982/1180448733805154405/image.png?ex=657d758d&is=656b008d&hm=7f59ba40dc9a7f4e97bafa14764d23cfb7d19f850992205831560e9353074ac5&)<br>

![Table](https://cdn.discordapp.com/attachments/1173915504872796160/1181950690961141761/image.png?ex=6582ec5c&is=6570775c&hm=c3cfee7e4c5bc8869fc8f09cbb3c7d2deb2c98fbf31af12dae8215cc8be93401&)<br>
Sesuai dengan table, netmask yang digunakan adalah /19 kemudian diturunkan terus hingga /30. Perlu diketahui jumlah node yang kosong harus sesuai dengan jumlah node yang ada per netmask.

### Tree
![treevlsm](https://cdn.discordapp.com/attachments/1173915504872796160/1180527123946012672/image.png?ex=657dbe8f&is=656b498f&hm=a2b9da7bd905317aa5c367ced25a5b59ea9fbf543ac8e097336ed58ef279b8a0&)

# CPT - CIDR

## Subneting

### Topologi CPT - CIDR
![Topology](https://cdn.discordapp.com/attachments/945123026410831952/1181950106480676985/FUCK_THIS_FUCKING_BULLSHIIIIIT_AAAAAAAAAAAAAAAA.png?ex=6582ebd0&is=657076d0&hm=df3b1595011832a472a0992f6044f4679efdf64c0cae95f5ab3a4e7dfc78ad52&)

### Tree CPT - CIDR
![Tree](https://cdn.discordapp.com/attachments/945123026410831952/1181950106912694383/tree_fix.png?ex=6582ebd1&is=657076d1&hm=59d265c3ce3926f2d62bbc97d4d54e85dc33ae9550cc31970b451d9b5249c206&)

### Subnet Table for CIDR
![Table](https://cdn.discordapp.com/attachments/945123026410831952/1181951005584265316/image.png?ex=6582eca7&is=657077a7&hm=dc04841cdf0716e5e449bcd76cfa8ffc19d8f6522bc77b54cc141d0a7b5f269d&)

Disclaimer! Prefix IP kelompok adalah 10.79, karena mask terakhir adalah /14 maka dibutuhkan banyaknya IP sehingga dalam perhitungan membutuhkan tambahan prefix sehingga menjadi 10.79 sampai 10.82

## IP Configurating

### A1 
#### Aura
![AuraA!](https://cdn.discordapp.com/attachments/945123026410831952/1181953538855800902/image.png?ex=6582ef03&is=65707a03&hm=d5bc7c50d085ff6e3c0788603ef955bf2374508bfc5f5221baeeebae4d39fb4f&)
#### Frieren
![FrierenA1](https://cdn.discordapp.com/attachments/945123026410831952/1181953842254979123/image.png?ex=6582ef4b&is=65707a4b&hm=42dfd5c151467adc0336d1695342d02600451e412e76028d3719ce78b4bb2db8&)
### A2
#### Aura
![AuraA2](https://cdn.discordapp.com/attachments/945123026410831952/1181954505416376360/image.png?ex=6582efe9&is=65707ae9&hm=575fe185f812466e018565f4f390499fb253b5f074fac8d78924e3b52e6062c6&)
#### Denken
![DenkenA2](https://cdn.discordapp.com/attachments/945123026410831952/1181954772715192482/image.png?ex=6582f029&is=65707b29&hm=8bd111939cf12e04a2efc176454757a5938e8ed8175174520507f57f977b59bc&)
### A3
### A4
### A5
### A6
### A7
### A8
### A9

## Routing 
### Aura
![RoutAura](https://cdn.discordapp.com/attachments/945123026410831952/1181955286035087491/image.png?ex=6582f0a3&is=65707ba3&hm=4797b4df6847b1549a6942e8a36c42b6c3ce1b02326f9b3e54c901b8d1465445&)
![RoutAura2](https://cdn.discordapp.com/attachments/945123026410831952/1181955439689220196/image.png?ex=6582f0c8&is=65707bc8&hm=2e067cb8abc56727bd9e575cacd27744e01b7da4994e0910476bbd49e7898bd5&)

### Frieren
![RoutFrieren](https://cdn.discordapp.com/attachments/945123026410831952/1181958085825286264/image.png?ex=6582f33f&is=65707e3f&hm=37abb63f14f2a3261f65d10788435c468b6569a3ab83c0b2abcf3025b8834ac4&)
### Denken
![RoutDenken](https://cdn.discordapp.com/attachments/945123026410831952/1181958312011501578/image.png?ex=6582f375&is=65707e75&hm=c4824ed3520007464f93f93987a1d7bef89239d28ee19722b1de9c9559edcac6&)
### Eisen
![RoutEisen](https://cdn.discordapp.com/attachments/945123026410831952/1181958471562821702/image.png?ex=6582f39b&is=65707e9b&hm=c8f73391b3f68c12d8e529e35e4a403b85e036495abdfad9fd945bf80c94437f&)
### Flamme
![RoutAura](https://cdn.discordapp.com/attachments/945123026410831952/1181958612055248997/image.png?ex=6582f3bc&is=65707ebc&hm=21b7799c4cdf351c15cb3c9dcfa7b699ab00fbefbb0c4db1d0eb20ad5609ed27&)
### Fern
![RoutFern](https://cdn.discordapp.com/attachments/945123026410831952/1181959042151747694/image.png?ex=6582f423&is=65707f23&hm=ebe2716d7b685eedb30ce788f733a063aa86a90e3079d89745de641e5db818b9&)
### Himmel
![RoutHimmel](https://cdn.discordapp.com/attachments/945123026410831952/1181959177887809670/image.png?ex=6582f443&is=65707f43&hm=c2500272c769b807aaf8d6577180304f2de05253dd671a14662a9acf43ee5769&)
### Linie
![RoutLinnie](https://cdn.discordapp.com/attachments/945123026410831952/1181959491915370586/image.png?ex=6582f48e&is=65707f8e&hm=684e7213878666c92f6208e0a3cb0539d05bead3e3304c287f8c1b13503594a1&)
### Lawine
![RoutLawine](https://cdn.discordapp.com/attachments/945123026410831952/1181959599507644436/image.png?ex=6582f4a8&is=65707fa8&hm=838acc91e15aa5f0af9e711f1708bb85ce56a113d9e4f780a3cebe7c9e7a4b30&)
### Heiter
![RoutHeiter](https://cdn.discordapp.com/attachments/945123026410831952/1181959718458118164/image.png?ex=6582f4c4&is=65707fc4&hm=bf768e15c834ca08c83a558841dbb6a7defbcde28791fb9f1341da9f6854a802&)
## Testing

Ping RohrRoad (10.80.240.2) Dari GranzChannel (10.81.32.2)

![Pingtest1](https://cdn.discordapp.com/attachments/945123026410831952/1181956818709262417/image.png?ex=6582f211&is=65707d11&hm=83eb36a370c0909ebc1076aa7a05340621b1d73009f17fc771b7799991beee70&)
![result1](https://cdn.discordapp.com/attachments/945123026410831952/1181957183974408233/image.png?ex=6582f268&is=65707d68&hm=d076b5b4d24c3369f0cf309684c8d4e1d2d675228d0aa938a344d18b595bf47c&)
