# **Klasifikacije slika limfnih čvorova za detekciju malignih tkiva**

Ovo je projekat radjen za predmet Mašinsko učenje na Matematičkom fakultetu Univerziteta u Beogradu. \
Zadatak je uporedjivanje klasičnog i dubokog pristupa klasifikaciji slika. 

Izvor podataka i inspiracija za projekat: https://patchcamelyon.grand-challenge.org. 

## **Uputstvo za skidanje fajlova**:
Zbog veličine, dataset fajlovi ne mogu biti okačeni na github-u.
Dostupni podaci (sa gore navedenog sajta) su u startu podeljeni na Train, Test i Validation fajlove, ali zbog prikaza postupaka, uzeti su Test fajlovi. \
Skinuti sa linka https://drive.google.com/drive/folders/1gHou49cA1s5vua2V5L98Lt8TiWA3FrKB sledeća dva fajla:
* camelyonpatch_level_2_split_test_x.h5.gz -> otpakovati -> preimenovati u **Camelyon_x.h5**
* camelyonpatch_level_2_split_test_y.h5.gz -> otpakovati -> preimenovati u **Camelyon_y.h5**

Voditi računa da treba da budu sačuvani u folderu 'dataset', jer je putanja za čitanje fajlova 'dataset/Camelyon_x.h5' i 'dataset/Camelyon_y.h5'

Izabrani su Test fajlovi zbog prihvatljive dimenzije, koja je takodje sa **32768** uzoraka smanjena na **12000** radi lakšeg treniranja modela. 

## **Klasični pristup**:
* Logistička regresija (*Logistic regression*)
* Slučajne šume (*Random forest*)
* K najbližih suseda (*KNN*)
* Stabla odlučivanja (*Decision trees*)
* Naivni Bayes (*Naive Bayes*)
* Metod potpornih vektora (*SVC*)
* Pojačavanje (Boosting):
  1. Ada Boost
  2. XGBoost
  3. Gradient Boost
* Prosta agregacija (*bagging*)

## **Duboki pristup**:
* Neuronske mreže (*ANN*)
* Konvolutivne neuronske mreže (*CNN*)
