# Botpress Test Application
## Exchange Rates ChatBot (Task)
Setup a chatbot on Botpress version 12.x and publish to Telegram via Botfather.

### Chatbot should provide the following features:
##### Today’s Exchange Rates for EUR:
* USD/EUR
* RUB/EUR
* RON/EUR
* GBP/EUR

##### Exchange Rate Variation in comparison with yesterday exchange rates (↑↓)
* USD: 17.30 ↑
* RUB: 19.20 ↓
* etc.

##### Exchange Rates calculator
* User select a currency
* Then input amount
* Chatbot shows all currencies amount equivalent with the sum introduced by the user
    * USD: 2.43
    * RUB: 2.2
    * Etc.

### Backend Features:

1.  Exchange rates to be consumed by this API:
    *  https://api.ratesapi.io/api/{Date}?base={base_currency}&symbols={to_Currency} (https://api.ratesapi.io/api/2021-04-06?base=RON&symbols=USD)

1. Saving Exchange Rates into Database.
    * All Requested Exchange Rates to be saved into Database so that next time user request Exchange Rates for already saved date into DB, chatbot will return rates from DB, otherwise from API.

1.  Knex migration for creating table where Exchange Rates will be saved.

### Front-End Features:
1.  Show Chatbot Users Metrics in Botpress Admin Panel:
    * Conversation count
    * Exchange Calculator Usage count

## Technology Stack
* Botpress v12.x
* Language: NodeJS/Typescript
* DataBase: Postgresql
* Platform: Docker
