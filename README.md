# Projrkt wykonany w grupie
## Cel projektu
Werykacja jakości materiałów jest bardzo ważnym elementem na każdym etapie cyklu produkcyjnego. Poprawne przeprowadzenie tej operacji ma duży wpływ na jakość produktu końcowego, a co za tym idzie, podnosi jego atrakcyjność i cenę. 

Celem projektu było opracowanie i implementacja algorytmu identyfikującego miejsce występowania wadliwej powierzchni i określającego jej wielkość na podstawie cyfrowego zdjęcia materiału.

## Opis algorytmu
  1. Wybór obrazu ze skazą - Obraz przedstawia drewnianą powierzchnię, na drewnie widać słoje oraz sęki. Sęki traktowane są jako skaza.

![image](https://user-images.githubusercontent.com/105323115/194776589-3b120153-6da4-409e-9698-14da7eae2b59.png)
  2. Zmiana kontrastu obrazu - Zmiana kontrastu obrazu jest konieczna do wyznaczenia intensywności poszczególnych pikseli. Później z tych intensywności zostanie wyrysowany histogram.

![image](https://user-images.githubusercontent.com/105323115/194776661-4bf8568c-686e-4286-b499-9fa841fde0e6.png)

Histogram przed zmianą kontrastu:

![image](https://user-images.githubusercontent.com/105323115/194776794-1022616e-68e0-471c-acc7-fead68f9bc30.png)

Histogram po zmianie kontrastu:

![image](https://user-images.githubusercontent.com/105323115/194776772-0f7f5775-5ace-4c52-a041-53ab55cb4f02.png)

  3. Zmiana obrazu z RGB na skalę szarości - Zmiana obrazu z kolorowego na skalę szarości jest podstawą do narysowania histogramu oraz ułatwieniem w przejściu na obraz  monochromatyczny.
  
![image](https://user-images.githubusercontent.com/105323115/194776829-caf122bb-a84a-47e6-9dcc-18809607771c.png)

  4. Zmiana obrazu ze skali szarości na obraz monochromatyczny - Korzystając z ustalonego granicznego proguprocentowego materiał zostaje oddzielony od skazy. Tło (materiał) zostaje zamieniony na kolor czarny, a skaza na biały.
  
![image](https://user-images.githubusercontent.com/105323115/194776875-78130a18-bc6e-44a9-b0f7-cf4e0629d22d.png)

  5. Wygładzanie krawędzi skazy przy użyciu operacji morfologicznej.
  
![image](https://user-images.githubusercontent.com/105323115/194776919-c391c451-d5a1-4de0-b037-3af2e6e668f4.png)

  6. Zaznaczenie na obrazie konturów skazy - Wyznaczone kontury skazy zostają naniesione na pierwotny obraz.
  
![image](https://user-images.githubusercontent.com/105323115/194776986-c2db274d-bfc5-4b70-8965-0a72a25a1626.png)

## Wypróbowanie programu na innych rodzajach materiałów: 
  1. ![image](https://user-images.githubusercontent.com/105323115/194777080-36407647-bfa5-4699-b4b9-726e51672a4b.png)
  ![image](https://user-images.githubusercontent.com/105323115/194777099-4aa38bdb-1987-4aac-85cc-652158bef728.png)

  2. ![image](https://user-images.githubusercontent.com/105323115/194777140-b3524391-1d05-471b-a0d5-4fd86b1902c1.png)
  ![image](https://user-images.githubusercontent.com/105323115/194777148-bcfd7b49-c667-455e-bb5b-cab3d925dbc0.png)
  
  3. ![image](https://user-images.githubusercontent.com/105323115/194777158-4fe773b2-74f8-4e5a-946b-cb89e03e2595.png)
  ![image](https://user-images.githubusercontent.com/105323115/194777167-8bf089b8-7461-49b9-b558-5f8ff4e85adf.png)

  4. ![image](https://user-images.githubusercontent.com/105323115/194777198-7a3d66b3-8830-44bb-b97c-19125ca5f25e.png)
  ![image](https://user-images.githubusercontent.com/105323115/194777208-a1c0a3fa-c019-4884-81db-2dd0256f630f.png)






