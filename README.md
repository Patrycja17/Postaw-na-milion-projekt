# Postaw-na-milion-projekt
projekt postaw na milion

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
    odpowiedz_gracza = input('Wpisz literę odpowiedzi:\n')
    if odpowiedz_gracza.lower() == i[1].lower():
        print('Prawidłowa odpowiedź.\n')
        wylos_kom_dobra_odp = random.choice(komentarze_dobra_odp)
        print(wylos_kom_dobra_odp)
    else:
        print('Błędna odpowiedź.\n')
        wylos_kom_zla_odp = random.choice(komentarze_zla_odp)
        print(wylos_kom_zla_odp)
