+++
title="Navodila za seminar pri predmetu Praktikum: Pisanje za elektronske medije"
date=2025-01-15

[extra]
author = "princessSarmica"
toc = true

[taxonomies]
categories = ["Seminar"]
tags = ["PPEM", "Navodila", "Trpljenje"]
+++

# Navodila za pripravo vsebine za objavo na spletni strani – Praktikum: Pisanje za elektronske medije  

Dragi sošolci,  

Kakorkoli se bo sledeč stavek glupo slišal, upam, da še niste preveč delali na seminarju, saj bi vam rad podal nekaj smernic za poenostavitev priprave vsebine in objavo na spletni strani (upam, da nisem too late 😥).

# Kaj je treba pripraviti?  
## 1. **Besedilo**  
   - Pripravite besedilno vsebino (približno 1000 besed) v formatu Word ali drugem tekstovnem formatu (npr. `.docx`, `.txt`, ali `.odt`).  
   - V dokument lahko vključite tudi opombe, kje želite dodati multimedijske elemente, kot so slike, videi, grafi itd.

## 2. **Slike**  
   - Pošljite slike ločeno od besedilnega dokumenta (npr. v formatu `.jpg` ali `.png`).  
   - Kak so slike poimenovane ni pomembno. 
   - Če boste imeli več slik je tudi možno oblikovanje v obliki fotogalerije 

{% galleria() %}
{
  "images": [
    {
      "src": "slika1.png",
      "title": "Lazanja 1",
      "description": "Njam."
    },
    {
      "src": "slika2.png",
      "title": "Lazanja 2",
      "description": "Njam."
    },
    {
      "src": "slika3.png",
      "title": "Lazanja 3",
      "description": "Njam."
    },
    {
      "src": "slika4.png",
      "title": "Lazanja 4",
      "description": "Njam."
    }
  ]
}
{% end %}

## 3. **Video vsebine**  
   - Najlažje je, če video naložite na YouTube in mi pošljete povezavo. YouTube link lahko vključite neposredno v besedilni dokument, kamor želite, da ga umestim.  

{{ youtube(id="KESyoPHt2kw") }}

## 4. **Grafikoni in infografike**  
   - Če želite vključiti grafikone, lahko podatke pripravite v Excelu, Wordu, ali čem podobnem in jih priložite. Če bi bilo možno, bi bil vesel, če mogoče grafikon izrišete, da dobim idejo, kako bi naj izgledal (da nebi npr. moral izgledati graf kot kvadratna funkcija, jaz bi pa na strani izrisal korensko funkcijo).  
   - Prav tako bi rad omenil, da bodo grafikoni na spletni strani avtomatsko lahko že interaktivni

V nadaljevanju sledi prikaz nekaj možnih interaktivnih grafikonov.

**Toti grafikon:**

{% chart() %}
{
"type": "Line",
"title": "Učenje povprečnega študneta",
"xLabel": "x",
"yLabel": "y",
"data": {
    "labels": ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10"],
    "datasets": [
    {
        "label": "Razmišljanje o učenju",
        "data": [30, 70, 200, 300, 500, 800, 1500, 2900, 5000, 8000]
    },
    {
        "label": "Dejansko učenje",
        "data": [0, 1, 30, 70, 80, 100, 50, 80, 40, 150]
    }
    ]
}
}
{% end %}  

**Toti drugi grafikon:**

{% chart() %}
{
  "type": "XY",
  "title": "Pokemon farme",
  "xLabel": "Koordinacija",
  "yLabel": "Količina",
  "data": {
    "datasets": [
      {
        "label": "Pikachu",
        "data": [
          {
            "x": 3,
            "y": 10
          },
          {
            "x": 4,
            "y": 122
          },
          {
            "x": 10,
            "y": 100
          }
        ]
      },
      {
        "label": "Squirtle",
        "data": [
          {
            "x": 1,
            "y": 1
          },
          {
            "x": 3,
            "y": 3
          }
        ]
      },
      {
        "label": "Charizard",
        "data": [
          {
            "x": 2,
            "y": 5
          },
          {
            "x": 6,
            "y": 8
          }
        ]
      }
    ]
  },
  "options": {
    "xTickCount": 5,
    "yTickCount": 5,
    "showLine": false,
    "dotSize": 1
  }
}
{% end %}

**Ta ta tretji grafikon:**

{% chart() %}
{
  "type": "Bar",
  "title": "Kako zapravin mesečno štipendijo",
  "xLabel": "Hudiči zapravljanja",
  "yLabel": "Denar (EUR)",
  "data": {
    "labels": ["študentski boni", "Pijača", "Muller"],
    "datasets": [
      {
        "data": [30, 45, 100]
      }
    ]
  },
  "options": {
    "yTickCount": 2,
    "dataColors": ["Red", "Green", "Blue"]
  }
}
{% end %}

**Še en grafikon**

{% chart() %}
{
  "type": "StackedBar",
  "title": "Sadje, ki ga prodajajo branjevke",
  "xLabel": "Branjevke",
  "yLabel": "Število sadja",
  "data": {
    "labels": ["Lojzka", "Petra", "Bukev", "Sara", "Balbina"],
    "datasets": [
      {
        "label": "Jabolka",
        "data": [12, 19, 11, 29, 17]
      },
      {
        "label": "Slive",
        "data": [3, 5, 2, 4, 1]
      },
      {
        "label": "Banane",
        "data": [2, 3, 0, 1, 1]
      }
    ]
  }
}
{% end %}

**Tortnii (yey za tega celo ven ime):**

{% chart() %}
{
  "type": "Pie",
  "title": "Priljubljenost tort med študenti",
  "data": {
    "labels": ["jagodna torta", "borovnična torta", "biskvit", "pinki torta", "pistacija myb?"],
    "datasets": [
      {
        "data": [500, 200, 80, 90, 100]
      }
    ]
  }
}
{% end %}

**Ka da f je to??! To sploh kdo uporabla??**

{% chart() %}
{
  "type": "Radar",
  "title": "???",
  "data": {
    "labels": ["c", "h", "a", "r", "t"],
    "datasets": [
      {
        "label": "???",
        "data": [2, 1, 1, 3, 1]
      },
      {
        "label": "???",
        "data": [1, 2, 2, 1, 1]
      }
    ]
  },
  "options": {
    "showLegend": true,
    "showLabels": true
  }
}
{% end %}

## 5. **Dodatni večpredstavnostni elementi**  
   - Možno je tudi vključiti zemljevide, zvočne posnetke ali druge interaktivne elemente.

# Predlog za čim bolj preprosto pripravo  
- Najpomembnejše je, da vsebino pripravite v čim bolj osnovni obliki. Poskrbeli bomo za prilagoditve in tehnično urejanje na spletni strani.  
- Če imate kakšno vprašanje, se lahko obrnete name 🐱

# Zaključek  
Skupaj lahko poskrbimo, da bodo vaše vsebine odlično izpadle na spletni strani. Ne pozabite, da je ključ do uspeha dobro pripravljeno besedilo in osnovni vizualni elementi – za vse drugo bomo poskrbeli med samim urejanjem. (To je rekel ChatGPT, ne jaz)  

Za samo vsebino, ki jo boste pripravili bi mogoče zaprosil edino še, da mi podate tudi nekaj naslovov za kategorije in tagge, po katerih je vaš članek zaznamovan (npr. kategorija Kulinarika, Zdrava prehrana; taggi: Lazanja, Garfiled, Fat Cat).

Also...pri temni temi sem opazil, da znajo slike in video posnetki dobiti čudno formo spektra barv, taka toti bug še morem odpravit.

Prispevke in vsebino oddajte v skupno mapo, pri čemer naj vsak par ustvari svojo podmapo, kamor bo shranil svoje gradivo. Povezava do skupne mape je na voljo v naši Messenger/Discord skupini.
Hvala vnaprej za sodelovanje in se veselim vaših prispevkov! 😊 

LPP in lep pozdrav,
princessSarmica
