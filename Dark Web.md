# Dark Web

## OnionSearch

**Description:** https://github.com/megadose/OnionSearch OnionSearch is a Python3 script that scrapes urls on different ".onion" search engines. The search engines they use are: 

ahmia
darksearchio
onionland
notevil
darksearchenginer
phobos
onionsearchserver
torgle
onionsearchengine
tordex
tor66
tormax
haystack
multivac
evosearch
deeplink

**Usage**
First we start Tor
```
service tor start
```

Then we verify its running with:
```
service tor status
```

Next we search for a key term using all search engines and using Tor proxy
```
onionsearch --proxy 127.0.0.1:9050 "Conti"
```

To request all the engines excepted "Ahmia" and "Candle" for the word "computer":
```
onionsearch "computer" --exclude ahmia candle
```

To request only "Tor66", "DeepLink" and "Phobos" for the word "computer":
```
onionsearch "computer" --engines tor66 deeplink phobos
```

The same as previously but limiting to 3 the number of pages to load per engine:
```
onionsearch "computer" --engines tor66 deeplink phobos --limit 3
```

## DarkDump
**Description** \
Darkdump is a simple script written in Python3.11 in which it allows users to enter a search term (query) in the command line and darkdump will pull all the deep web sites relating to that query. Darkdump2.0 is here, enjoy! \
**Install**
```
git clone https://github.com/josh0xA/darkdump
cd darkdump
python3 -m pip install -r requirements.txt
python3 darkdump.py --help
```
**Usage**
```
python3 darkdump.py --query programming
```
```
python3 darkdump.py --query="chat rooms"
```
```
python3 darkdump.py --query hackers --amount 12
```
**Proxy Usage**
```
python3 darkdump.py --query bitcoin -p
```
**Help**
```
usage: darkdump.py [-h] [-v] [-q QUERY] [-a AMOUNT] [-p]

options:
  -h, --help            show this help message and exit
  -v, --version         returns darkdump's version
  -q QUERY, --query QUERY
                        the keyword or string you want to search on the deepweb
  -a AMOUNT, --amount AMOUNT
                        the amount of results you want to retrieve (default: 10)
  -p, --proxy           use darkdump proxy to increase anonymity

```



## Search

**onion.live** https://onion.live/ \
**Demon** http://srcdemonm74icqjvejew6fprssuolyoc2usjdwflevbdpqoetw4x3ead.onion/ \
**Excavator** http://2fd6cemt4gmccflhm6imvdfvli3nf7zn6rfrwpsy7uhxrgbypvwf5fad.onion/ \
**Fresh Onions** http://freshonifyfe4rmuh6qwpsexfhdrww7wnt5qmkoertwxmcuvm4woo4ad.onion/ \
**Kilos** http://mlyusr6htlxsyc7t2f4z53wdxh3win7q3qpxcrbam6jf3dmua7tnzuyd.onion/search \
**Onion Center** http://5qqrlc7hw3tsgokkqifb33p3mrlpnleka2bjg7n46vih2synghb6ycid.onion/ \
**Hidden Reviews** http://u5lyidiw4lpkonoctpqzxgyk6xop7w7w3oho4dzzsi272rwnjhyx7ayd.onion/ \
**Onionland** http://3bbad7fauom4d6sgppalyqddsqbf5u5p56b5k5uk2zxsy3d6ey2jobad.onion/ \
**Phobos** http://phobosxilamwcg75xt22id7aywkzol6q6rfl2flipcqoc4e4ahima5id.onion/ \
**Recon** http://recon222tttn4ob7ujdhbn3s4gjre7netvzybuvbq2bcqwltkiqinhad.onion/ \
**Submarine** http://no6m4wzdexe3auiupv2zwif7rm6qwxcyhslkcnzisxgeiw6pvjsgafad.onion/ \
**The Deep Searches** http://searchgf7gdtauh7bhnbyed4ivxqmuoat3nm6zfrg3ymkq6mtnpye3ad.onion/ \
**Tor66** http://tor66sewebgixwhcqfnp5inzp5x5uohhdy3kvtnyfxc2e5mxiuh34iid.onion/ \
**Torch** http://torchqsxkllrj2eqaitp5xvcgfeg3g5dr3hr2wnuvnj76bbxkxfiwxqd.onion/ \
**Torch Links** http://torchlu7soq4akgqojbby4fgfwsxyppjdlzry2qtn7lbghfalxurbjad.onion/



## Ransomware

**RansomDB** https://www.ransom-db.com/ \
**Ransomlook** https://www.ransomlook.io/ and excellent site that actually lists what these blogs are posting as well as screenshots of the blog page \
**Ransomlook** https://www.ransomlook.io/ \
**Ransom Watch** https://ransomwatch.telemetry.ltd/#/INDEX \
**Ransomwatch Feed** https://raw.githubusercontent.com/joshhighet/ransomwatch/main/posts.json \
**RansomChat** https://ransomch.at/ A site that shows the contents of ransomware chats, like them talking to their victims \
**RansomPosts** https://privtools.github.io/ransomposts/. Another site tracking ransomware blog posts of victims. \
**DecryptTools** https://www.nomoreransom.org/en/decryption-tools.html Ransomware decryption tools \
**Ransomware Decrypt** https://www.avast.com/en-gb/ransomware-decryption-tools#. Avast's list of ransomware decryption tools and fixes \
**Ransomware Group Sites Index** http://ransomwr3tsydeii4q43vazm7wofla5ujdajquitomtd47cxjtfgwyyd.onion/ \
**Lorenz** http://lorenzmlwpzgxq736jzseuterytjueszsvznuibanxomlpkyxk6ksoyd.onion/ \
**Omega** http://omegalock5zxwbhswbisc42o2q2i54vdulyvtqqbudqousisjgc7j7yd.onion/ \
**Alphv 1** http://alphvmmm27o3abo3r2mlmjrpdmzle3rykajqc5xsj7j7ejksbpsa36ad.onion/?page=1 \
**Alphv 2** http://vqifktlreqpudvulhbzmc5gocbeawl67uvs2pttswemdorbnhaddohyd.onion/search \
**Avos Locker** http://avosqxh72b5ia23dl5fgwcpndkctuzqvh2iefk5imp3pi5gfhel5klad.onion/ \
**Babuk** http://nq4zyac4ukl4tykmidbzgdlvaboqeqsemkp4t35bzvjeve6zm2lqcjid.onion/ \
**BianLian** http://bianlianlbc5an4kgnay3opdemgcryg2kpfcbgczopmm3dnbz3uaunad.onion/ \
**Cheers** http://rwiajgajdr4kzlnrj5zwebbukpcbrjhupjmk6gufxv6tg7myx34iocad.onion/ \
**Clop** http://santat7kpllt6iyvqbr7q4amdv6dzrh6paatvyrzl7ry3zm72zigf4ad.onion/ \
**Conti** http://santat7kpllt6iyvqbr7q4amdv6dzrh6paatvyrzl7ry3zm72zigf4ad.onion/ \
**Conti Torrents** http://toznnag5o3ambca56s2yacteu7q7x2avrfherzmz4nmujrjuib4iusad.onion/ \
**Cuba** http://cuba4ikm4jakjgmkezytyawtdgr2xymvy6nvzgw5cglswg3si76icnqd.onion/ \
**Daixin** http://7ukmkdtyxdkdivtjad57klqnd3kdsmq6tp45rrsxqnu76zzv3jvitlqd.onion/ \
**Everest** https://ransomocmou6mnbquqz44ewosbkjk3o5qjsl3orawojexfook2j7esad.onion.ly/ \
**Free Civilian** http://gcbejm2rcjftouqbxuhimj5oroouqcuxb2my4raxqa7efkz5bd5464id.onion/ \
**Lockbit** http://lockbitapt2yfbt7lchxejug47kmqvqqxvvjpqkmevv4l3azl3gy6pyd.onion/ \
**Lockbit** http://lockbitaptc2iq4atewz2ise62q63wfktyrl4qtwuk5qax262kgtzjqd.onion/ \
**Lockbit** http://lockbitapt34kvrip6xojylohhxrwsvpzdffgs5z4pbbsywnzsbdguqd.onion/ \
**Lockbit** http://lockbitapt6vx57t3eeqjofwgcglmutr3a35nygvokja5uuccip4ykyd.onion/ \
**Lockbit** http://lockbitapt5x4zkjbcqmz6frdhecqqgadevyiwqxukksspnlidyvd7qd.onion/ \
**Lockbit** http://lockbitapt2d73krlbewgv27tquljgxr33xbwwsp6rkyieto7u4ncead.onion/ \
**LV** http://rbvuetuneohce3ouxjlbxtimyyxokb4btncxjbo44fbgxqy7tskinwad.onion/ \
**Moses Staff** https://moses-staff.se/ \
**Payload.bin** http://vbmisqjshn4yblehk2vbnil53tlqklxsdaztgphcilto3vdj4geao5qd.onion/ \
**Ragnar Locker** http://rgleaktxuey67yrgspmhvtnrqtgogur35lwdrup4d3igtbm3pupc4lyd.onion/ \
**Ransomexx** http://rnsm777cdsjrsdlbs4v5qoeppu3px6sb2igmh53jzrx7ipcrbjz5b2ad.onion/ \
**Ransom House** http://xw7au5pnwtl6lozbsudkmyd32n6gnqdngitjdppybudan3x3pjgpmpid.onion/ \
**Red Alert** http://blog2hkbm6gogpv2b3uytzi3bj5d5zmc4asbybumjkhuqhas355janyd.onion/ \
**Snatch** http://hl66646wtlp2naoqnhattngigjp5palgqmbwixepcjyq5i534acgqyad.onion/index.php \
**SolidBit** http://solidb2jco63vbhx4sfimnqmwhtdjk4jbbgq7a24cmzzkfse4rduxgid.onion/login \
**Vice Society** http://vsociethok6sbprvevl4dlwbqrzyhxcxaqpvcqt5belwvsuxaxsutyad.onion/ \
**SunCrypt** http://x2miyuiwpib2imjr5ykyjngdu7v6vprkkhjltrk4qafymtawey4qzwid.onion/ \
**Yanulang** http://jukswsxbh3jsxuddvidrjdvwuohtsy4kxg2axbppiyclomt2qciyfoad.onion/ \
**Qilin** http://kbsqoivihgdmwczmxkbovk7ss2dcynitwhhfu5yw725dboqo5kthfaad.onion/ \
**Royal** http://royal4ezp7xrbakkus3oofjw6gszrohpodmdnfbe5e4w3og5sm7vb3qd.onion/ \
**BlackByte** http://jbeg2dct2zhku6c2vwnpxtm2psnjo2xnqvvpoiiwr5hxnc6wrp3uhnad.onion/ \
**VSOP** http://mrdxtxy6vqeqbmb4rvbvueh2kukb3e3mhu3wdothqn7242gztxyzycid.onion/ \
**Dunghill** http://p66slxmtum2ox4jpayco6ai3qfehd5urgrs4oximjzklxcol264driqd.onion/index.html \
[Ransom Wiki](https://ransom.wiki) Check if your company or vendors were in a ransomware breach.

## Miscellaneous
[Dark Mirror](https://socradar.io/labs/darkmirror) \
[Anonymous Blogging](http://anonblogd4pcarck2ff6qlseyawjljaatp6wjq6rqpet2wfuoom42kyd.onion/) \
[Board of Shame](http://blog2hkbm6gogpv2b3uytzi3bj5d5zmc4asbybumjkhuqhas355janyd.onion/) \
[Dark Leak Market](http://darkleakyqmv62eweqwy4dnhaijg4m4dkburo73pzuqfdumcntqdokyd.onion/) \
[AlphaBay](http://alphabay522szl32u4ci5e3iokdsyth56ei7rwngr2wm7i5jo54j2eid.onion/) \
[Dark Web Journal](http://tdef74zmruajphutbzuqlxzpi5btckiypgpfmug6bl235e4mn6xarvad.onion/tdwj/) \
[Tape news](http://tape6m4x7swc7lwx2n2wtyccu4lt2qyahgwinx563gqfzeedn5nb4gid.onion/) \
[Evil Corp Marketplace](http://castlee5janmtc5h6jiorit7lzdhgfuy43po4oddgi3qpm52ljyljyyd.onion/) \
[XSS Forum](http://xssforumv3isucukbxhdhwz67hoa5e2voakcfkuieq4ch257vsburuid.onion/) \
[Flashlight 2.0 News](http://ovgl57qc3a5abwqgdhdtssvmydr6f6mjz6ey23thwy63pmbxqmi45iid.onion/) \
[Anonymous Hackers](http://twcd7fo4eepxznx7vajl5njkfpkz3g3z6qhynffcy3hb6n42dov2omid.onion/) \
[Tox Chat](https://tox.chat/) Seems to be the most popular messaging being used by ransomware groups \
[Leaked Wiki](https://leaked.wiki) Seems to be a lot of pastes of things like stealer logs and stuff. \
[Nulled Blog](nullbulge.se/blog.html) Clearnet blog for a group called Nulled. \
[BreachForum Search](https://bf.based.re/) A site that you can search by Breach Forum users and view all of their posts. \
[DarkMirror](https://socradar.io/labs/darkmirror/) SocRadars Dark Web news blog. \
[Tor Socks](https://github.com/dgoulet/torsocks) Torify your applications. \
[TOR Exit Nodes](https://check.torproject.org/torbulkexitlist) Tor exit nodes \
[TOR Exit Nodes 2](https://www.dan.me.uk/tornodes) Another Tor exit node list \
[TorBot](https://github.com/MikeMeliz/TorCrawl.py) A Tor Crawler \
[Darknet Dictionary](https://darkweblink.com/darknet-dictionary/) A site for information on terms used in the dark web. \
[Tor exit node list](https://www.dan.me.uk/tornodes) List of Tor exit nodes. \
[Dark Owl](https://www.darkowl.com/blog-content/) Dark Web blog \
[Tor Metrics](https://metrics.torproject.org) Different Tor metrics


## Forums
**Blackforums** https://blackforums.net/ \
**BlackForums2** https://blackforums.me/ \
**Breached** http://breachedu76kdyavc6szj6ppbplfqoz3pgrk3zw57my4vybgblpfeayd.onion/ \
**Dread** http://dreadytofatroptsdj6io7l3xptbet6onoyno2yv7jicoxknyazubrad.onion/ \
**Exploit.in** https://exploitivzcm5dawzhe6c32bbylyggbjvh5dyvsvb5lkuz5ptmunkmqd.onion/ \
**Leakbase** https://leakbase.io/ \
**Nulled** https://www.nulled.to/ \
**XSS** http://xssforumv3isucukbxhdhwz67hoa5e2voakcfkuieq4ch257vsburuid.onion/ \


