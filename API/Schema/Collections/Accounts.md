```json
{
	"_id": "NumerRachunku(string)"
	"currencies?": [
		{
			"currency": "waluta",
			"amount": "float"
		},
		{}
	]
	"loans?": [
		{
			"startedAt": "date",
			"endsAt": "date",
			"lentAmount": "float",
			"totalToPay": "float",
			"monthInstallment(rata)": "float",
			"installments": [
				{
					"_id": "number of installment"
					"amount": "float",
					"amountLeftToPay": "float",
					"paymentDate(data do kiedy trzeba zapłacic)": "date",
					"paidAt": "date/null"
				}
			]
			"interest(odsetki za zwłokę)": "float",
			"autoPayment": "boolean"
		}
	],
	"standingOrders(przelewy cykliczne)?": [
		{
			"title": "string",
			"to": "NumerRachunku",
			"nextPayment": "date - can be past date if failed",
			"lastPaymentFailed": "boolean",
			"currency": {
				"currency": "waluta",
				"amount": "float"
			}
		}
	],
	"savedRecipients": [
		"accountNumber": "NumerKonta",
		"recipientName(wpisane przez użytkownika)": "String"
	],
	"cryptoAccountInfo": {
		"accountLevel": "int (1-10)",
		"levelProgress": "int (do uzgodnienia, kazdy level iles trzeba kupic/sprzedac)",
		"dollarsTr	aded": "float"
	}
}
```
NumerRachunku - "CC AAAA AAAA BBBB BBBB BBBB BBBB":
*	CC - suma kontrolna
*	AAAA AAAA - numer rozliczeniowy banku
*	BBBB BBBB BBBB BBBB - numer konta. Dwie pierwsze cyfry wezmy jako 01 - konto standardowe, 02 - wielowalutowe, 03 - kryptowalutowe

Waluta - najlepiej Enum obiektów. Pamiętać, że konta mogą zawierać tylko niektóre waluty.
