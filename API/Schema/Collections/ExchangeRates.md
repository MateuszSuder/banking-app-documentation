```json
{
	type: "fiat",
	exchangeRates: [
		{
			currency: "string (USD/PLN/EUR...) / ENUM?",
			price: "float"
		}
	],
	defaultCurrency: "USD/PLN/EUR"
},
{
	type: "crypto",
	exchangeRates: [
		{
			currency: "string (BTC/ETH/LTC...) / ENUM?",
			price: "float",
			withdrawFee*: "float"
		},
		defaultCurrency: "USDT/BTC/ETH"
	],
}
```

Kilka dokumentów dla różynch walut????? Chyba nie mozemy do zewnętrzengo api wysylc duzo requestow bo bedzie trzeba placić, dlatego lepiej w bazie to trzymać