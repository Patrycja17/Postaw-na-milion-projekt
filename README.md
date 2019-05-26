# Postaw-na-milion-projekt
projekt postaw na milion

from random import sample
import random
import time

print("Witaj w grze POSTAW NA MILION")
print("Na starcie masz do dyspozycji 1000000 zł.")
print("Możesz je rozkładać na dowolnie wybrane odpowiedzi, ale jedna z nich zawsze musi pozostać pusta.")
print("Masz minutę na obstawianie odpowiedzi.")
print("Zaczynamy!")

Pytania_4odp = ['Czarny charakter w "Królu Lwie" Disneya miał na imię:\n a. Rafiki    |     b. Skaza\n c. Mufasa    |     d. Aslan',
             'Jakie miasto jest stolicą Kazachstanu?\n a. Astana     |     b. Ałmaty\n c. Baku     |     d. Biszkek ',
             'Żółta łódź podwodna to statek:\n a. Beatlesów     |     b. Doorsów\n c. Pearl Jamu    |     d. Joy Division ',
             'Kim była Ariel z filmu Disneya?\n a. Elfem     |     b. Wróżką\n c. Rusałką     |     d. Syrenką ',
             '"Czynnik" to składnik\n a. Sumy     |     b. Dzielenia\n c. Mnożenia     |     d. Pierwiastkowania ',
             'Który z tych posągów jest najwyższy\n a. Pomnik Lenina z Wołgogradzie     |     b. Statua Wolności w Nowym Jorku\n c. Chrystus Król w Świebodzinie     |     d. Wielki Sfinks w Gizie ',
             'Skąd jest najbliżej do Gdańska w linii prostej?\n a. z Warszawy     |     b. ze Szczecina\n c. z Poznania     |     d. z Wrocławia ',
             'Czego było więcej?\n a. Dalmatyńczyków     |     b. Prac Heraklesa\n c. Lat samotności (u Marqueza)     |     d. Upadków Bunga (u Witkacego) ',
             ]
Odpowiedzi_4odp = ['b',
           'a',
           'a',
           'd',
           'c',
           'b',
           'c',
           'd',
           ]


komentarze_dobra_odp = ['Dobra robota.\n',
           'Idziemy do przodu.\n',
           'Świetnie ci idzie.\n'
           ]

komentarze_zla_odp = ["No niestety.\n",
            "Następnym razem będzie lepiej.\n",
            "Proszę się nie martwić.\n"]

key = list(zip(Pytania_4odp, Odpowiedzi_4odp)) 

s = sample(key, 4) 

for i in s:
    print(i[0])
    print("Czas na odpowiedź:")
    for x in range(60, 0, -1):
        print(x, end='\r')
        time.sleep(1)
    odpowiedz_gracza = input('Wpisz literę odpowiedzi:\n')
    if odpowiedz_gracza.lower() == i[1].lower():
        print('Prawidłowa odpowiedź.\n')
        wylos_kom_dobra_odp = random.choice(komentarze_dobra_odp)
        print(wylos_kom_dobra_odp)
    else:
        print('Błędna odpowiedź.\n')
        wylos_kom_zla_odp = random.choice(komentarze_zla_odp)
        print(wylos_kom_zla_odp)
        
Pytania_3odp = ['Który z królów Polski panował najdłużej?\n a. Bolesław Chrobry    |     b. Władysław Jagiełło\n c. Zygmunt III Waza     |     d. ',
             '"Wściekłe psy", "Pulp fiction" to dzieła:\n a. braci Coen     |     b. Jamesa Camerona\n c. Quentina Tarantino     |     d. ',
             'Największy dzwon w Polsce usłyszeć można w:\n a. Krakowie     |     b. Toruniu\n c. Licheniu     |     d. ',
             'Nigel Kennedy gra na:\n a. Stratocasterze     |     b. Stradivariusie\n c. Steinwayu     |     d. ',
             'Clifford to wielki czerwony\n a. bocian     |     b. pies\n c. kot     |     d. ',
             'Cięciwa okręgu może być:\n a. promieniem     |     b. średnicą\n c. styczną     |     d. ',
             '"Spadać w dół" i "cofać się do tyłu" to przykłady błędów językowych zwanych potocznie masłem maślanym. Jaka jest ich fachowa nazwa?\n a. Polisyndeton     |     b. Pleonazm\n c. Epifraza     |     d. ',
             'Skąd dokąd płynął Titanic w swym dziewiczym rejsie?\n a. Z Southampton do Nowego Jorku     |     b. Z Liverpoolu do Nowego Jorku\n c. Z Londynu do Southampton     |     d. ',
             ]

Odpowiedzi_3odp = ['b',
           'c',
           'c',
           'b',
           'b',
           'b',
           'b',
           'c',
           ]


komentarze_dobra_odp2 = ['Jesteśmy już w drugim etapie.\n',
           'Coraz bliżej do miliona.\n',
           'Proszę się nie stresować.\n'
           ]

komentarze_zla_odp2 = ["Żegnam.\n",
            "I pieniążki przepadły.\n"
            ]


key = list(zip(Pytania_3odp, Odpowiedzi_3odp)) 
s = sample(key, 3) 

for i in s:
    print(i[0])
    print("Czas na odpowiedź:")
    for x in range(60, 0, -1):
        print(x, end='\r')
        time.sleep(1)
    odpowiedz_gracza = input('Wpisz literę odpowiedzi:\n')
    if odpowiedz_gracza.lower() == i[1].lower():
        print('Prawidłowa odpowiedź.\n')
        wylos_kom_dobra_odp2 = random.choice(komentarze_dobra_odp2)
        print(wylos_kom_dobra_odp2)
    else:
        print('Błędna odpowiedź.\n')
        wylos_kom_zla_odp2 = random.choice(komentarze_zla_odp2)
        print(wylos_kom_zla_odp2)

Pytania_2odp = ['Jaka grecka litera widnieje w logo Wikipedii\n a. omega    |     b. alfa\n c.     |     d. ',
             'Drzwi, których skrzydło przy otwieraniu obraca się zgodnie z ruchem wskazówek zegara to:\n a. drzwi prawe     |     b. drzwi lewe\n c.      |     d. ',
             'Aby uwolnić się z Matrixa Neo wybrał pigułkę w kolorze:\n a. niebieskim     |     b. czerwonym\n c.      |     d. ',
             'Który z tych aktorów "zginął" na planie więcej razy?\n a. Mel Gibson     |     b. Robert De Niro\n c.      |     d. ',
             ]

