# Master-of-Orion-TTS-Prototype-
Projec in LUA scripts

### Opis projektu  
W ramach projektu moim zadaniem było opracowanie mechaniki rozstawiania początkowego obiektów na stole do gry, co miało znacząco ułatwić i przyspieszyć rozpoczęcie rozgrywki. Realizacja mechanizmu opierała się na identyfikacji obiektów z dedykowanych worków frakcji za pomocą unikalnych identyfikatorów (**ID**). Po pobraniu obiektu gracz mógł umieścić go na planszy w odpowiedniej pozycji, przypisanej do konkretnego gracza na podstawie danych z tablicy pozycji.  

Aby zwiększyć elastyczność i ułatwić zarządzanie kodem, utworzyłem ukryty obiekt, pełniący rolę "biblioteki", w której przechowywałem funkcje wykorzystywane w innych częściach projektu. Dzięki temu mechanika stała się bardziej modularna i czytelna.  

### Dodatkowe funkcjonalności  
1. **Losowanie i wybór frakcji:** Dodałem przyciski umożliwiające losowanie frakcji zgodnie z instrukcją, a także wybór konkretnej frakcji oraz jej resetowanie do worka, by umożliwić ponowne wybory.  
2. **Automatyzacja:** Stworzyłem funkcję pozwalającą na dodanie automy do gry. Mechanizm ten wybiera oraz blokuje wybraną frakcję (lub dwie frakcje) w taki sposób, by nie mogły być wybrane przez graczy, co było zgodne z instrukcją gry. Ostatecznie te frakcje są rozstawiane na stole w miejscach przeznaczonych na automy. 

### Wyzwania i rozwiązania  
Jednym z większych wyzwań było przekazanie tablicy wielowymiarowej między funkcjami znajdującymi się w różnych obiektach. Wymagało to dokładnego zrozumienia struktury języka **LUA** oraz sposobu, w jaki funkcje komunikują się między sobą w środowisku projektu.  

Dodatkowym wyzwaniem była nauka samego języka **LUA**, z którym wcześniej nie miałem doświadczenia. W ciągu tygodnia opanowałem tworzenie funkcji, zarządzanie danymi oraz odwoływanie się do obiektów za pomocą **ID**.  

### Refleksja  
Praca nad tym projektem była dla mnie cennym doświadczeniem. Oprócz nauki nowego języka programowania, zdobyłem również umiejętności w testowaniu mechanik i modularnym podejściu do kodu. Choć projekt wymaga jeszcze optymalizacji, udało się osiągnąć założone cele, w tym poprawę funkcjonalności i wygody rozgrywki.  

---

### Project Description  
In this project, my task was to develop a mechanic for setting up initial objects on the game table, significantly simplifying and speeding up the game start process. The implementation was based on identifying objects from dedicated faction bags using unique identifiers (**ID**). Once an object was retrieved, players could place it on the board in a position assigned to them based on data from a position table.  

To enhance flexibility and make the code easier to manage, I created a hidden object acting as a "library," where I stored functions used in other parts of the project. This approach made the mechanics more modular and easier to maintain.  

### Additional Features  
1. **Faction randomization and selection:** I added buttons that allow players to randomize factions according to the game’s rules, choose specific factions, or reset them back to the bag for another selection.  
2. **Automation:** I implemented a function that introduces an "automa" (AI-controlled player) into the game. This mechanism selects and blocks the chosen faction (or two factions) so that they cannot be picked by other players, adhering to the game’s rules. Finally, these factions are automatically placed on the table in positions designated for automas.  

### Challenges and Solutions  
One of the main challenges was passing a multidimensional array between functions located in different objects. Overcoming this required a solid understanding of the **LUA** language and how functions interact within the project's environment.  

Another challenge was learning **LUA** itself, as I had no prior experience with it. Within a week, I managed to grasp the basics of creating functions, handling data, and referencing objects using **ID**.  

### Reflection  
This project was a valuable learning experience. Beyond mastering a new programming language, I gained skills in testing mechanics and adopting a modular approach to coding. While the project could benefit from further optimization, the primary goals were successfully achieved, improving both functionality and the overall gameplay experience.  
