# Bounding_Boxes_for_CAA_Wilhelmshaven
Code and Bounding Boxes model done for CAA Wilhelmshaven 2019 (https://ag-caa.de/workshop2019/)

# Installation:
Beside the files from this repository you need to download the following model files:

Save to /model folder:

https://drive.google.com/file/d/1-rAm-ZL_5clG3QUJapuSgUT9sm4tvI9a/view?usp=sharing

https://drive.google.com/file/d/1Jf1hfkArNk3uiZzYL7fE7I6dH5L7O0uT/view?usp=sharing

Save to /model/saved_model folder (has to be created):

https://drive.google.com/file/d/1mNRdHKoPnB0srAT7YQYcj4TEexRDOp1e/view?usp=sharing

# Bounding Boxes als Werkzeug zur Trennung von Porträt und Inschrift auf Bildern von antiken römischen Münzen

Keywords: Object Detection, Bounding Boxes, Image Recognition, Convolutional Neural Network, Ancient Coins

# Abstract: 

Wir arbeiten an einem Machine Learning Modell zur Identifizierung römischer Kaiser auf antiken Münzen. Dazu verwenden wir aktuell ein Bilderkennungsmodell auf Grundlage eines Convolutional Neural Networks. Das Training und die Tests wurden auf der Online Coins of the Roman Empire und der Corpus Nummorum Thracorum Datenbank ausgeführt. Unser Ziel ist es das Modell weiter zu verbessern.
Die Auswertung der bisherigen Ergebnisse unter Verwendung der vollständigen Münzvorderseite mit Porträt und Inschrift als Grundlage des Trainings, führt dazu, dass eine Münze mit Porträt teilweise oder vollständig anhand der Inschrift klassifiziert wird (trifft bei mehr als 50% der getesteten Münzen zu). Um dieses Problem zu lösen, haben wir die ML Methode der automatischen Erstellung einer Bounding Box angewandt. Hierbei lernt ein vortrainiertes Object Detection Modell durch einen weiteren Trainingsschritt den Porträtbereich einer Münze zu erkennen. Dafür haben wir ein auf einem Regional Convolutional Neural Network basierendes Modell für das Training und das Tool LabelImg zur Annotation benutzt.
Eine Herausforderung in diesem Rahmen ist es, das möglichst vollständige Porträt mit so wenig Inschrift wie möglich innerhalb der Box liegen zu haben. Auch der Umgang mit durch Abrieb beschädigte oder beim Prägevorgang verrutschte Porträts muss erlernt werden. Im nächsten Schritt sollen die Porträts innerhalb der Box ausgeschnitten werden und als neue Trainingsdaten für das Bilderkennungsmodell dienen.
Dieses Modell ist eine aktualisierte Version des in Wilhelmshaven gezeigten Modells. Besonders das Verhalten bei aus der Münzmitte beim Prägevorgang verrutschten Porträts wurde verbessert.

