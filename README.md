# ERD - Diagram Związków Encji

## Entity Relationship Diagram (ERD)
ERD to graficzny sposób reprezentacji związków pomiędzy encjami. Poprawnie zbudowany diagram powinien zawierać encje, ich atrybuty oraz związki między nimi.

---

## 📌 Encja
Encja określa różnego rodzaju obiekty lub wydarzenia. Na diagramach reprezentowana jest jako **prostokąt**. Z technicznego punktu widzenia opisuje "magazyny danych" – dlatego nazwę w takim prostokącie umieszcza się u góry, stosując **rzeczownik w liczbie mnogiej**.

---

## 📌 Atrybut
Atrybut to cecha charakterystyczna encji – w implementacji informatycznej odpowiada polom w bazie danych. 

- Atrybuty są zapisywane w kolejnych wierszach w ramach encji.
- Ich nazwy zazwyczaj zapisuje się w **liczbie pojedynczej**.
- Specyficznym atrybutem jest **unikatowy identyfikator** (**klucz główny**), który jednoznacznie identyfikuje rekord w bazie.
- Jeśli w tabeli nie ma pojedynczego pola pozwalającego na unikatową identyfikację wpisu, stosuje się **identyfikator sztuczny**, najczęściej pole `ID`.

---

## 📌 Relacje
Relacje pomiędzy encjami mogą mieć różne typy:

- **1:1** – jedna encja jest powiązana dokładnie z jedną inną encją.
- **1:n** – jedna encja może być powiązana z wieloma encjami.
- **m:n** – wiele encji może być powiązanych z wieloma innymi encjami.

Każda relacja może posiadać dodatkową cechę – **opcjonalność**, która określa minimalną liczebność relacji:
- `0` – oznacza opcjonalność (brak wymaganego powiązania),
- `1` – oznacza obowiązkowe wystąpienie relacji.

---

## 🛠 Proces Projektowania Bazy Danych
Cały proces projektowania bazy danych składa się z trzech podstawowych faz:

### 🔍 1. Analiza wymagań
Pierwszy etap obejmuje:
- Wywiady z interesariuszami,
- Analizę wymagań biznesowych,
- Określenie zadań, jakie projektowana baza ma usprawnić.

🔹 **Nie istnieje jednoznaczna odpowiedź na pytanie „Jak prowadzić analizę wymagań?”** – istnieją różne metody, które pomagają określić wymagania biznesowe.

---

### 📌 2. Realizacja koncepcyjnego modelu logicznego
Drugi etap polega na stworzeniu **logicznego modelu bazy danych** na podstawie wcześniejszej analizy. 
- W tym kroku modelowane są wszystkie encje, atrybuty i związki w postaci **diagramu ERD**.

---

### 💾 3. Modelowanie fizycznego modelu i implementacja bazy
Ostatni etap obejmuje **implementację rzeczywistej bazy danych** na podstawie stworzonego modelu ERD.

---

📌 **Podsumowanie**
ERD jest kluczowym narzędziem do projektowania baz danych, pozwalającym na wizualne przedstawienie encji, ich atrybutów i związków pomiędzy nimi. Proces projektowania bazy obejmuje analizę wymagań, modelowanie logiczne oraz fizyczne, które prowadzą do finalnej implementacji systemu.
