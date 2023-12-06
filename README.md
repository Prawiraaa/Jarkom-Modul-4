
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

## CPT - CIDR
### Topologi CPT - CIDR
![Topology](https://cdn.discordapp.com/attachments/945123026410831952/1181950106480676985/FUCK_THIS_FUCKING_BULLSHIIIIIT_AAAAAAAAAAAAAAAA.png?ex=6582ebd0&is=657076d0&hm=df3b1595011832a472a0992f6044f4679efdf64c0cae95f5ab3a4e7dfc78ad52&)

### Tree CPT - CIDR
![Tree](https://cdn.discordapp.com/attachments/945123026410831952/1181950106912694383/tree_fix.png?ex=6582ebd1&is=657076d1&hm=59d265c3ce3926f2d62bbc97d4d54e85dc33ae9550cc31970b451d9b5249c206&)

### Subnet Table for CIDR
![Table](https://cdn.discordapp.com/attachments/945123026410831952/1181951005584265316/image.png?ex=6582eca7&is=657077a7&hm=dc04841cdf0716e5e449bcd76cfa8ffc19d8f6522bc77b54cc141d0a7b5f269d&)

Disclaimer! Prefix IP kelompok adalah 10.79, karena mask terakhir adalah /14 maka dibutuhkan banyaknya IP sehingga dalam perhitungan membutuhkan tambahan prefix sehingga menjadi 10.79 sampai 10.82
