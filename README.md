# definiciju_vardnica
# Projekta darbs "Vārdu skaidrojumu atrašanas automatizēšana"
# Veidotājs : Marta Terēze Jurjāne
# Apliecības nr : 221RWC046

# Programmas teorijas un izpildes apraksts:
(Programma sākotnēji izveidota Visual Studio Code)
Īsi sakot, projekta darba ietvaros izveidotā programma automatizē vārdu skaidrojumu izgūšanu no Tezaurs virtuālās vārdnīcas. Lai varētu tikt uzsākts programmas izpildes process, tiek pieprasīts iepriekš izveidots excel fails ar neierobežotu skaitu latviešu vārdu faila 'A' kolonnā, kas tiek atvērts un pa rindiņai nolasīts, izmantojot bibliotēkas "openpyxl" Workbook un load_workbook rīkus. Izmantojot vairākus "selenium" bibliotēkas webdriver rīkus tiek definēts, ka tiks atvērta https://tezaurs.lv saite tieši Chrome pārlūkprogrammā. Elementi secīgi tiek ievadīti saites meklēšanas lodziņā un to skaidrojums tiek atgriezts programmai,  kas savukārt to ievada 'B' kolonnā jaunizveidotā excel failā, kas, papildus jauniegūtajām definīcijām, satur arī iepriekšesošā vārdu saraksta excel faila informāciju. Tiek veikta arī kļūdu pārbaude ar "selenium" rīku NoSuchElementException - gadījumā, ja kāds no definējamajiem vārdiem neatrodas https://tezaurs.lv vārdnīcas krātuvē, programma jaunizveidotajā failā attiecīgajā "Nozīme" ailē ievadīs tekstu "Tezaurā šim vārdam skaidrojuma nav".
Programma ir viegli izmaināma gadījumā, ja ir interese definēt citu valodu vārdus, jo izpildes princips paliek salīdzinoši līdzīgs: nepieciešams specifiski definēta excel faila formāta vārdu saraksts, virtuālās vārdnīcas web saite un attiecīgās "selenium" bibliotēkai veicamās darbības, lai programma varētu atgriezt derīgu skaidrojumu.
