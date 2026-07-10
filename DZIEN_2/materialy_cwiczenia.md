# Materiały do ćwiczeń promptowych

---

## ĆWICZENIE 1 — Reklamacja z ograniczeniami

**Zadanie:** Napisz prompt, który wygeneruje odpowiedź na poniższą reklamację. Warunki: ton uprzejmy, ale bez nadmiernego przepraszania, maksymalnie 4 zdania, jedno konkretne rozwiązanie.

**Materiał wejściowy — treść reklamacji:**

> Zamówiłem u Państwa ekspres do kawy 8 dni temu z opcją dostawy "do 48 godzin". Paczka do dziś nie dotarła, a status przesyłki nie zmienił się od czwartku. Dzwoniłem dwa razy na infolinię — za pierwszym razem czekałem 20 minut i się rozłączyło, za drugim usłyszałem, że "sprawa jest w toku". Potrzebuję tego ekspresu na prezent, który wręczam w sobotę. Albo dostanę konkretną informację kiedy paczka dotrze, albo proszę o zwrot pieniędzy i anulowanie zamówienia.

**Kryterium oceny:** Czy prompt wymusza wszystkie trzy ograniczenia jednocześnie i nie pozwala modelowi rozlać się w ogólniki.

---

## ĆWICZENIE 2 — Ekstrakcja strukturalna

**Zadanie:** Napisz prompt, który z poniższej notatki wyciągnie: decyzje, osoby odpowiedzialne i terminy. Output wyłącznie jako czysty JSON — bez komentarza, bez znaczników markdown.

**Materiał wejściowy — notatka ze spotkania:**

> Spotkanie zespołu produktowego, wtorek rano. Ustaliliśmy w końcu, że nową wersję panelu klienta wypuszczamy 15 marca — Kasia bierze na siebie koordynację wdrożenia i ma przygotować checklistę do końca tego tygodnia. Marek marudził, że testy nie są gotowe, więc zgadaliśmy o tym dłużej i wyszło, że QA musi skończyć regresję do 10 marca, inaczej ślizgamy się z datą. Padła też decyzja, żeby nie ruszać na razie integracji z płatnościami — Tomek to odkłada na drugi kwartał, wraca do tematu po świętach. A, i jeszcze: Ania ogarnia komunikację do klientów, mailing wychodzi dzień przed premierą, czyli 14 marca. Ktoś rzucił pomysł webinaru, ale nikt tego nie podjął, więc zostawiamy w zawieszeniu.

**Test poprawności:** Czy wygenerowany output da się od razu sparsować jako JSON (bez ręcznego czyszczenia).

---

## ĆWICZENIE 3 — Przełożenie rejestru

**Zadanie:** Napisz jeden prompt, który wygeneruje trzy warianty poniższego komunikatu dla trzech odbiorców: zarząd (zwięźle, strategicznie), zespół techniczny (konkretnie), klient (bez żargonu). Wyzwanie: rozdzielić trzy rejestry w jednym promcie bez ich zlania.

**Materiał wejściowy — komunikat bazowy:**

> Migracja systemu do nowej infrastruktury chmurowej zakończyła się sukcesem. W trakcie prac wystąpiła nieplanowana przerwa w dostępności usługi trwająca 40 minut w nocy z soboty na niedzielę. Wszystkie dane zostały w pełni zachowane. Nowa infrastruktura zapewnia szybsze ładowanie i większą stabilność przy dużym obciążeniu. Koszt utrzymania spada o około 30% w skali roku. W kolejnym etapie planowane jest wdrożenie automatycznego skalowania.

**Kryterium oceny:** Czy każdy z trzech wariantów faktycznie mówi językiem swojego odbiorcy i czy prompt wymusza ich rozdział, a nie trzy niemal identyczne akapity.
