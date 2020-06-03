# Bounding_Boxes_for_CAA_Wilhelmshaven
Code and Bounding Boxes model done for CAA Wilhelmshaven 2019 (https://ag-caa.de/workshop2019/)


# Bounding Boxes als Werkzeug zur Trennung von Portr�t und Inschrift auf Bildern von antiken r�mischen M�nzen

Keywords: Object Detection, Bounding Boxes, Image Recognition, Convolutional Neural Network, Ancient Coins

Abstract: 

Wir arbeiten an einem Machine Learning Modell zur Identifizierung r�mischer Kaiser auf antiken M�nzen. Dazu verwenden wir aktuell ein Bilderkennungsmodell auf Grundlage eines Convolutional Neural Networks. Das Training und die Tests wurden auf der Online Coins of the Roman Empire und der Corpus Nummorum Thracorum Datenbank ausgef�hrt. Unser Ziel ist es das Modell weiter zu verbessern.
Die Auswertung der bisherigen Ergebnisse unter Verwendung der vollst�ndigen M�nzvorderseite mit Portr�t und Inschrift als Grundlage des Trainings, f�hrt dazu, dass eine M�nze mit Portr�t teilweise oder vollst�ndig anhand der Inschrift klassifiziert wird (trifft bei mehr als 50% der getesteten M�nzen zu). Um dieses Problem zu l�sen, haben wir die ML Methode der automatischen Erstellung einer Bounding Box angewandt. Hierbei lernt ein vortrainiertes Object Detection Modell durch einen weiteren Trainingsschritt den Portr�tbereich einer M�nze zu erkennen. Daf�r haben wir ein auf einem Regional Convolutional Neural Network basierendes Modell f�r das Training und das Tool LabelImg zur Annotation benutzt.
Eine Herausforderung in diesem Rahmen ist es, das m�glichst vollst�ndige Portr�t mit so wenig Inschrift wie m�glich innerhalb der Box liegen zu haben. Auch der Umgang mit durch Abrieb besch�digte oder beim Pr�gevorgang verrutschte Portr�ts muss erlernt werden. Im n�chsten Schritt sollen die Portr�ts innerhalb der Box ausgeschnitten werden und als neue Trainingsdaten f�r das Bilderkennungsmodell dienen.

