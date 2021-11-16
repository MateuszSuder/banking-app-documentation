
Funkcjonalności:
* Zakładanie konta użytkownika
	* Rejestracja - Front (Auth0)
	* Potwierdzenie maila (*) - Front (Auth0)
	* Otrzymanie kodów do potwierdzania transkacji na maila - [[verification-codes]]
* Zakładanie kont
	* Konta standardowe 
	* Konta wielowalutowe
	* Konto kryptowalutowe
* Autoryzacja i autentykacja (Standard oAuth2, platforma Auth0)
	* Token JWT
		* Otrzymanie tokena
		* Walidacja tokena (pod zwgledem autentykacji i autoryzacji)
		* Odświeżanie tokena
		* Unieważnianie tokena
	* Prawa użytkowników
* Przelewy
	* Przelewy standardowe między istniejącymi kontami bankowymi
		* Wymagany jest kod z podanym numerem (kody potwierdzające z maila)
		* Walidacja danych
	* Przelewy cykliczne
		* Możliwość ustawienia przelewu co jakiś czas
		* Przypomnienie w aplikacji dla użytkownika po zalogowaniu w czasie ustalonym przed
	* Historia przelewów
	* Wyciąg bankowy (CSV)
* Pożyczki bankowe
	* Możliwość wzięcia kredytu
	* Do wyboru spłata automatyczna lub manualna
	* Rosnące odsetki przez spóźnienia
* Zapisani odbiorcy
	* Dodawanie nowych odbiorców (Dla tych odbiorców nie trzeba podawać kodu mailowego)
	* Usuwanie odbiorców
* Konto wielowalutowe
	* Możliwość wpłaty z każdego konta w banku
	* Zamiana jednostek
	* Wypłaty w danej walucie
	* Dane o walucie z api(*)
* Konto kryptowalutowe
	* Możliwość wpłaty w zł oraz między innymi kontami kryptowalutowymi
	* Możliwość kupna oraz sprzedaży kryptowalut
	* Prowizja za przewalutowanie
	* Wypłaty tylko w zł
	* Stopnie konta
		* Każda transakcja podwyższa poziom konta
		* Wyższy poziom konta - mniejsze prowizje
	* Dane o kryptowalutach z api(*)
	* Wykresy walut(*)
	* Anonimowa lista transkacji kryptowalut z banku(*)