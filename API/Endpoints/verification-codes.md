# Verification codes
*Służy do wysłania na maila kodów użytkownika*

**Wymaga autoryzacji: Tak**

```
Mając - Dane o użytkowniku i rodzaj konta, do którego konta mają zostać wysłane
Kiedy - Kiedy użytkownik zapyta o kody
Wtedy - Wygeneruj i/lub wyślij na maila kody
```

Przebieg:
1. Zbierz id konta oraz mail użytkownika
2. Sprawdź czy kody dla tego użytkownika istnieją
	1. Jeżeli nie istnieją
		1. Wygeneruj kody składające się z cyfr (8 cyft np 12345678 LOSOWE)
		2. Przypisz je do indeksów
		3. Zapisz w bazie
3. Wyślij kody użytkownikowi

Co można użyc:
* [[Mailer]]