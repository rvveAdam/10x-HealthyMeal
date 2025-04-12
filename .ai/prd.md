# Dokument wymagań produktu (PRD) - HealthyMeal

## 1. Przegląd produktu

HealthyMeal to aplikacja przeglądarkowa, która umożliwia użytkownikom dostosowywanie przepisów kulinarnych do ich osobistych potrzeb i preferencji żywieniowych przy wsparciu sztucznej inteligencji. Aplikacja pozwala użytkownikom na przeglądanie przepisów, modyfikowanie ich składników za pomocą AI, dodawanie własnych przepisów oraz filtrowanie dostępnych dań według różnych kryteriów.

Główne funkcje produktu:
- System kont użytkowników z pełnym zarządzaniem (rejestracja, logowanie, edycja, usuwanie)
- Katalog przepisów z dedykowanej bazy danych oraz możliwość dodawania własnych
- Inteligentne modyfikacje przepisów z propozycjami zamienników składników
- Zaawansowane filtrowanie przepisów według preferencji (słodkie/słone, kaloryczność, poziom trudności)
- System oceniania przepisów w skali 1-5 gwiazdek

Produkt jest przeznaczony dla osób, które chcą gotować posiłki dostosowane do ich specyficznych potrzeb żywieniowych, ale mają trudności z samodzielnym modyfikowaniem przepisów lub znajdowaniem odpowiednich zamienników składników.

## 2. Problem użytkownika

Użytkownicy zmagają się z następującymi problemami, które rozwiązuje HealthyMeal:

1. Trudność w modyfikowaniu istniejących przepisów w celu dostosowania ich do osobistych preferencji żywieniowych lub ograniczeń (alergie, nietolerancje)
2. Problemy ze znalezieniem odpowiednich zamienników składników, które zachowają smak i wartości odżywcze dania
3. Brak prostego sposobu filtrowania przepisów według własnych preferencji żywieniowych
4. Trudność w określeniu kaloryczności zmodyfikowanych przepisów
5. Brak możliwości przechowywania i organizowania przepisów dostosowanych do własnych potrzeb

Użytkownicy często rezygnują z gotowania według przepisów, które znaleźli, ponieważ nie odpowiadają one ich preferencjom lub ograniczeniom dietetycznym. HealthyMeal rozwiązuje ten problem, oferując inteligentne dostosowanie przepisów i proponowanie zamienników, które odpowiadają potrzebom użytkownika.

## 3. Wymagania funkcjonalne

### 3.1. System kont użytkowników
- Rejestracja użytkownika (e-mail, hasło)
- Logowanie użytkownika
- Zmiana hasła
- Usuwanie konta
- Edycja preferencji żywieniowych (alergie, kaloryczność, preferencje smakowe, podział na słone/słodkie)

### 3.2. Zarządzanie przepisami
- Przeglądanie katalogu przepisów
- Dodawanie własnych przepisów (do 5 na użytkownika)
- Modyfikowanie składników przepisów na własne potrzeby
- Proponowanie zamienników składników przez AI (do 5 pozycji)
- Ocenianie przepisów w skali 1-5 gwiazdek

### 3.3. Wyszukiwanie i filtrowanie
- Filtrowanie przepisów według kategorii (słodkie/słone)
- Filtrowanie przepisów według kaloryczności
- Filtrowanie przepisów według poziomu trudności

### 3.4. Szczegóły przepisu
- Wyświetlanie czasu przygotowania
- Lista składników
- Kroki przygotowania
- Kaloryczność (z marginesem błędu około 100 kcal)
- Poziom trudności
- Średnia ocen użytkowników

### 3.5. Interfejs użytkownika
- Responsywny design działający na urządzeniach mobilnych i desktopowych
- Minimalistyczny, prosty interfejs
- Wyświetlanie przepisów w formie kafelków z miniaturkami

## 4. Granice produktu

### 4.1. Co produkt będzie robić
- Umożliwiać zarządzanie kontem użytkownika
- Prezentować katalog przepisów z możliwością filtrowania
- Umożliwiać modyfikację przepisów i proponowanie zamienników składników
- Pozwalać na dodawanie własnych przepisów (z limitem 5 na użytkownika)
- Zapewniać system oceniania przepisów
- Działać jako aplikacja przeglądarkowa z responsywnym designem
- Korzystać z biblioteki open-source

### 4.2. Czego produkt nie będzie robić
- Nie będzie wysyłać powiadomień do użytkowników
- Nie będzie umożliwiać dodawania więcej niż 5 własnych przepisów na użytkownika
- Nie będzie umożliwiać edycji całych przepisów, tylko składników
- Nie będzie zapewniać funkcji społecznościowych (dzielenie się przepisami, komentowanie, itp.)
- Nie będzie działać jako aplikacja mobilna (tylko jako responsywna strona www)
- Nie będzie zapewniać informacji o dostępności składników w sklepach
- Nie będzie oferować planowania posiłków na wiele dni

## 5. Historyjki użytkowników

### US-001
**Tytuł**: Rejestracja nowego użytkownika

**Opis**: Jako nowy użytkownik, chcę utworzyć konto w aplikacji, aby móc korzystać z jej funkcjonalności.

**Kryteria akceptacji**:
1. Użytkownik może wprowadzić swój adres e-mail i hasło
2. System weryfikuje poprawność adresu e-mail i siłę hasła
3. Po pomyślnej rejestracji, użytkownik jest przekierowany do formularza preferencji żywieniowych
4. W przypadku błędu, system wyświetla odpowiednie komunikaty

### US-002
**Tytuł**: Logowanie do aplikacji

**Opis**: Jako zarejestrowany użytkownik, chcę zalogować się do aplikacji, aby uzyskać dostęp do moich ustawień i przepisów.

**Kryteria akceptacji**:
1. Użytkownik może wprowadzić swój adres e-mail i hasło
2. System weryfikuje poprawność danych logowania
3. Po pomyślnym logowaniu, użytkownik jest przekierowany do strony głównej
4. W przypadku błędnych danych, system wyświetla odpowiedni komunikat
5. Istnieje opcja "Zapomniałem hasła"

### US-003
**Tytuł**: Zmiana hasła

**Opis**: Jako zalogowany użytkownik, chcę zmienić moje hasło, aby zwiększyć bezpieczeństwo mojego konta.

**Kryteria akceptacji**:
1. Użytkownik może wprowadzić aktualne hasło oraz nowe hasło (dwukrotnie)
2. System weryfikuje poprawność aktualnego hasła i siłę nowego hasła
3. Po pomyślnej zmianie hasła, system wyświetla potwierdzenie
4. W przypadku błędu, system wyświetla odpowiednie komunikaty

### US-004
**Tytuł**: Usunięcie konta

**Opis**: Jako zalogowany użytkownik, chcę usunąć moje konto, aby moje dane nie były przechowywane w systemie.

**Kryteria akceptacji**:
1. Użytkownik może wybrać opcję usunięcia konta w ustawieniach
2. System wymaga potwierdzenia operacji poprzez wprowadzenie hasła
3. Po potwierdzeniu, konto i wszystkie dane użytkownika są trwale usuwane
4. Użytkownik jest wylogowywany i przekierowany na stronę główną z komunikatem o pomyślnym usunięciu konta

### US-005
**Tytuł**: Ustawienie preferencji żywieniowych

**Opis**: Jako użytkownik, chcę określić moje preferencje żywieniowe, aby otrzymywać przepisy dostosowane do moich potrzeb.

**Kryteria akceptacji**:
1. Użytkownik może wprowadzić informacje o alergiach (pole tekstowe)
2. Użytkownik może określić preferowaną kaloryczność posiłków
3. Użytkownik może wybrać preferencje smakowe
4. Użytkownik może określić preferencje dotyczące słodkich/słonych posiłków
5. System zapisuje preferencje i wykorzystuje je do personalizacji przepisów

### US-006
**Tytuł**: Przeglądanie katalogu przepisów

**Opis**: Jako zalogowany użytkownik, chcę przeglądać dostępne przepisy, aby znaleźć interesujące mnie posiłki.

**Kryteria akceptacji**:
1. Użytkownik widzi kafelki z miniaturkami przepisów na stronie głównej
2. Każdy kafelek zawiera podstawowe informacje o przepisie (nazwa, czas przygotowania, poziom trudności, kaloryczność)
3. Przepisy są wyświetlane w formie siatki, dostosowującej się do rozmiaru ekranu
4. Użytkownik może przewijać listę przepisów w celu zobaczenia większej liczby pozycji

### US-007
**Tytuł**: Filtrowanie przepisów

**Opis**: Jako zalogowany użytkownik, chcę filtrować przepisy według moich preferencji, aby łatwiej znaleźć odpowiednie posiłki.

**Kryteria akceptacji**:
1. Użytkownik może filtrować przepisy według kategorii (słodkie/słone)
2. Użytkownik może filtrować przepisy według zakresu kaloryczności
3. Użytkownik może filtrować przepisy według poziomu trudności
4. Filtry można łączyć ze sobą
5. Lista przepisów jest aktualizowana na bieżąco zgodnie z zastosowanymi filtrami

### US-008
**Tytuł**: Wyświetlanie szczegółów przepisu

**Opis**: Jako zalogowany użytkownik, chcę zobaczyć szczegóły przepisu, aby przygotować posiłek.

**Kryteria akceptacji**:
1. Użytkownik może kliknąć na kafelek przepisu, aby zobaczyć jego szczegóły
2. Szczegóły zawierają: nazwę, zdjęcie, czas przygotowania, poziom trudności, kaloryczność, składniki i kroki przygotowania
3. Wyświetlana jest również średnia ocena przepisu
4. Składniki są wylistowane z podaniem ilości
5. Kroki przygotowania są ponumerowane i wyświetlane w czytelnej formie

### US-009
**Tytuł**: Modyfikacja składników przepisu przez AI

**Opis**: Jako zalogowany użytkownik, chcę zmodyfikować składniki przepisu przy pomocy AI, aby dostosować go do moich preferencji żywieniowych.

**Kryteria akceptacji**:
1. Użytkownik może wybrać opcję modyfikacji przepisu na stronie szczegółów
2. Użytkownik może wskazać składniki, które chce zastąpić
3. System proponuje do 5 zamienników dla każdego składnika
4. Użytkownik może zaakceptować lub odrzucić propozycje
5. Po zaakceptowaniu zmian, system aktualizuje przepis z nowymi składnikami i dostosowuje kaloryczność

### US-010
**Tytuł**: Dodawanie własnego przepisu

**Opis**: Jako zalogowany użytkownik, chcę dodać własny przepis, aby móc go przechowywać i udostępniać w aplikacji.

**Kryteria akceptacji**:
1. Użytkownik może dodać do 5 własnych przepisów
2. Formularz dodawania przepisu zawiera pola: nazwa, zdjęcie, czas przygotowania, poziom trudności, kaloryczność, składniki, kroki przygotowania
3. System weryfikuje poprawność wprowadzonych danych
4. Po dodaniu przepisu, jest on widoczny w katalogu jako przepis użytkownika
5. System informuje, gdy limit 5 przepisów zostanie osiągnięty

### US-011
**Tytuł**: Ocenianie przepisu

**Opis**: Jako zalogowany użytkownik, chcę ocenić przepis, aby wyrazić swoją opinię o nim.

**Kryteria akceptacji**:
1. Użytkownik może ocenić przepis w skali 1-5 gwiazdek
2. Ocena jest zapisywana w systemie
3. Średnia ocen przepisu jest aktualizowana
4. Użytkownik może zmienić swoją ocenę
5. System nie pozwala na wielokrotne ocenianie tego samego przepisu przez jednego użytkownika

### US-012
**Tytuł**: Edycja składników na własne potrzeby

**Opis**: Jako zalogowany użytkownik, chcę edytować składniki przepisu na własne potrzeby, bez ingerencji AI.

**Kryteria akceptacji**:
1. Użytkownik może ręcznie edytować składniki przepisu
2. Edycja nie zmienia oryginalnego przepisu, tylko tworzy wersję dla użytkownika
3. Zmiany są zapisywane tylko dla danego użytkownika
4. System oznacza przepis jako zmodyfikowany przez użytkownika

## 6. Metryki sukcesu

### 6.1. Metryki zaangażowania użytkowników
- 90% użytkowników posiada wypełnioną sekcję preferencji żywnościowych
- 75% użytkowników generuje jeden lub więcej przepisów w tygodniu
- Średni czas spędzony w aplikacji wynosi co najmniej 5 minut na sesję
- Co najmniej 50% użytkowników wraca do aplikacji w ciągu tygodnia od pierwszego użycia

### 6.2. Metryki jakości
- Średnia ocena przepisów modyfikowanych przez AI wynosi co najmniej 4.0 na 5.0
- Mniej niż 10% użytkowników usuwa swoje konto w ciągu miesiąca od rejestracji
- Mniej niż 5% użytkowników zgłasza problemy z interfejsem użytkownika

### 6.3. Metryki wydajności
- Strona ładuje się w ciągu 3 sekund dla 95% użytkowników
- Generowanie propozycji zamienników przez AI zajmuje mniej niż 5 sekund
- System obsługuje jednocześnie co najmniej 100 użytkowników bez spadku wydajności 