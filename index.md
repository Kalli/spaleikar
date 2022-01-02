---
layout: home
title: ""
---

# Hvað eru spáleikar?

Spáleikar eru íslensk útgáfa af svokölluðum "_forecasting tournaments_". Ef þú vilt spreyta þig í að spá fyrir um atburði stjórnmálalíf, efnahagsmálum, viðskiptum, heilbrigðismálum og fleiru getur þú skoðað [spurningalistann og tekið þátt hér](https://docs.google.com/spreadsheets/d/1OSpBpLzgGRZkIADOaxeFkpIvFQDgIAkQYLtEWm2Ahpk/edit?usp=sharing) ([lestu leiðbeiningarnar](/spaleikar/leidbeiningar)). Öllum er frjálst að taka þátt, undir nafni eða nafnlaust. Eftir því sem líður á árið munum við svo sjá hverjir voru skarpastir í að spá fyrir atburðum ársins og í byrjun árs 2023 getum við verðlaunað völvu ársins 2022.

Í spáleikum gefa þátttakendur sér líkindi á að atburðir á opinberum vettvangi muni eiga sér stað innan gefins tímabils. Að leikunum loknum er gert upp hversu oft þátttakendur höfðu rétt fyrir sér og hvert hlutfall réttra svara var í hlutfalli við gefinn líkindi. Með líkindunum gefum við svigrúm, af því að það er erfitt að spá fyrir um framtíðina og eðlilegt að fólki bregðist stundum bogalistinn og sömuleiðis er líklegt að stundum giski maður einfaldlega á rétt svar. Með því að safna saman útkomum við gefinn líkindi getum við metið forspárgildi fólks með því að dæma hversu vel stilltar spár þeirra eru (e. *calibrated*).

## Hvað er reynt að spá fyrir um?

Spádómarnir geta verið af ólíku tagi. En við leitumst við að smíða spurningar sem hægt er að svara með nákvæmum, hlutlægu og afgerandi máta. Þar sem það er hægt er vísað í þriðja aðila sem heimild til úrskurðar. Hér eru nokkur dæmi:

* Katrín Jakobsdóttir verður forsætisráðherra Íslands 01.01.2023.
* Lið úr Vesturdeild NBA verður NBA meistari 2022.
* Heildar andlát vegna Covid-19 á Íslandi verða fleiri en 50 í lok árs 2022. 
* S&P 500 vísitalan verður hærri enn 5000 stig 01.01.2023.

## Hvernig er stigagjöf háttað?

Tökum sem dæmi veðurfræðing sem spáir 70% líkum á rigningu á morgun. Ef hann svo hangir þurr daginn eftir myndu margir segja að veðurfræðingurinn hafi haft rangt fyrir sér. En er það svo? Veðurfræðingurinn gaf sér að í aðstæðum dagsins myndi í þrem skiptum af tíu ekki falla dropi af himni. Réttara væri að finna 100 daga þar sem veðurfræðingurinn hefur spáð 70% líkindum á rigningu og gá hvort hann hafi haft rétt fyrir sér í um það bil 70 skipti.

Yfir fleiri spádóma má meta nákævmni spágildi með svokallaðari [Brier stigagjöf](https://en.wikipedia.org/wiki/Brier_score) (næstu málsgreinar er tiltölulega tæknilegar, ekki er nauðsynlegt að skilja þær í þaula til þess að taka þátt í spáleikunum). Brier stig er hittnifervik (e. *mean squared error*) þ.e. meðalgildi ferningstölu mismunar á spágildi og mældu gildi.

Ef við höldum áfram með dæmið af veðurfræðingnum auðmjúka[^1], þar sem annað hvort rignir (1) eða ekki (0) og þá mætti lýsa Brier stigagjöf fyrir nokkur spálíkindi sem svo:


| Spálíkindi    | Rignir | Útreikningur | Brier stig |
| ----------- | ----------- | ----------- | ----------- | ----------- |
| 100%      | Já  (1)     | (1-1)<sup>2</sup> = 0 | 0 (besta mögulega skor) |
| 100%      | Nei  (0)     | (1-0)<sup>2</sup> = 1 | 1 (versta mögulega skor) |
| 70%      | Já  (1)     | (0.7-1)<sup>2</sup> = 0.09 | 0.09 |
| 70%      | Nei  (0)     | (0.7-0)<sup>2</sup> = 0.49 | 0.49 |
| 50%      | Skiptir ekki máli     | (0.5-0)<sup>2</sup> = (0.5-1)<sup>2</sup> = 0.25 | 0.25 |

Þegar svör berast við spurningunum okkar getum við því reiknað út stig hvers leikmanns og reiknað út meðaltal þeirra. Líkt og í golfi leitast leikmaður því eftir að lágmarka Brier stigin sín. Í stigagjöfinni er þátttakendum refsað fyrir bæði að skjóta undir eða yfir, á meðan 50/50 spádómar eru svo til hlutlausir (og segja því lítið til um hæfileika þátttakenda).

Ef meðal Brier skorið manns er minna en 0.25 er maður sannspárri enn hreinar ágiskanir.


## Spáleikar 2022

Þessa dagana erum við að taka saman spurningar fyrir Íslenska spáleika 2022. Þú getur skoðað [drögin að spurningalistanum hér](https://docs.google.com/spreadsheets/d/1OSpBpLzgGRZkIADOaxeFkpIvFQDgIAkQYLtEWm2Ahpk/edit?usp=sharing) og leiðbeiningarnar um þáttöku [hér](/spaleikar/leidbeiningar)

Ef þú vilt senda inn spurningu geturðu sent tölvupóst ktryggvason(hjá)gmail.com, haft samband við [@karltryggvason](https://twitter.com/karltryggvason) á Twitter.

Við stefnum á að loka útgáfa spurningalistans verði tilbúinn 10. janúar 2022 og þátttakendur verða að skila inn endanlegum svörum sínum fyrir 1. Febrúar 2022.


---

[^1]: Dæmið er þýtt og staðfært af ensku færslunni fyrir [Brier Score](https://en.wikipedia.org/wiki/Brier_score#Example) á Wikipedia.