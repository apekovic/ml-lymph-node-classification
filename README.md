# **Klasifikacije slika limfnih čvorova za detekciju malignih tkiva**

Ovo je projekat radjen za predmet Mašinsko učenje na Matematičkom fakultetu Univerziteta u Beogradu. \
Zadatak je uporedjivanje klasičnog i dubokog pristupa klasifikaciji slika. 

Izvor podataka i inspiracija za projekat: https://patchcamelyon.grand-challenge.org. 

Dostupni podaci su u startu podeljeni na Train, Test i Validation fajlove, ali zbog prikaza postupaka, uzeti su Test fajlovi i preimenovani u:
* Camelyon_x.h5
* Camelyon_y.h5 

Izabrani su Test fajlovi zbog prihvatljive dimenzije, koja je takodje sa **32768** uzoraka smanjena na **12000** radi lakšeg treniranja modela. 

## **Klasični pristup**:
* Logistička regresija (*Logistic regression*)
* Slučajne šume (*Random forest*)
* K najbližih suseda (*KNN*)
* Stabla odlučivanja (*Decision trees*)
* Naivni Bayes (*Naive Bayes*)
* Metod potpornih vektora (*SVC*)

## **Neuspešni pokušaji naprednijih modela klasičnog pristupa koji nisu uspeli da budu testirani i popravljani, već su samo zakomentarisani**:
* Pojačavanje (*boosting*)
  1. Ada Boost
  2. XGBoost
  3. Gradient Boost
* Prosta agregacija (*bagging*)

## **Duboki pristup**:
* Neuronske mreže (*ANN*)
* Konvolutivne neuronske mreže (*CNN*)
