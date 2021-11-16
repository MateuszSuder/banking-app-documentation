```json
{
	_id: "NumerRachunku(string)"
	currencies: [
		{
			currency: "waluta",
			amount: "float"
		},
		{}
	],
	codes: [
		{
			_id: "int (1-8)"
			code: "int (8 digits)"
		}
	],
	loans: [
		{
			currency: "waluta",
			amount: "float",
			startedAt: "date",
			monthInstallment(rata): "int",
			interest(odsetki za zwłokę): "int",
			autoPayout: "boolean"
		}
	] 
}
```
NumerRachunku - "CC AAAA AAAA BBBB BBBB BBBB BBBB":
*	CC - suma kontrolna
*	AAAA AAAA - numer rozliczeniowy banku
*	BBBB BBBB BBBB BBBB - numer konta. Dwie pierwsze cyfry wezmy jako 01 - konto standardowe, 02 - wielowalutowe, 03 - kryptowalutowe

Waluta - najlepiej Enum obiektów. Pamiętać, że konta mogą zawierać tylko niektóre waluty.