# Botpress Test Application
## Exchange Rates ChatBot (Task)
Setup a chatbot on Botpress version 10.x and publish to Telegram via Botfather.

### Chatbot should provide the following features:
##### Today’s Exchange Rates for
* BNM – Banca Nationala
* CARD – Rate carduri
* PSV - Casa schimb valutar
* VIR - Virament

##### Exchange Rate Variation in comparison with yesterday exchange rates (↑↓)
* USD: 17.30 ↑
* EUR: 19.20 ↓
* etc.

##### Exchange Rates calculator
* User select a currency
* Then input amount
* Chatbot shows all currencies amount equivalent with the sum introduced by the user
    * USD: 2.43
    * EUR: 2.2
    * Etc.

### Backend Features:

1.  Exchange rates to be consumed by this API:
    *  [http://pki.maib.md/rates/CODyyyyMMdd.json](https://www.google.com/url?q=http://pki.maib.md/rates/CODyyyyMMdd.json&sa=D&ust=1584094197112000)
        * COD
            * BNM – Banca Nationala
            * CARD – Rate carduri
            * PSV - Casa schimb valutar
            * VIR - Virament
        * yyyyMMdd - data solicitare
Eg.:[http://pki.maib.md/rates/CARD20190211.json](https://www.google.com/url?q=http://pki.maib.md/rates/CARD20190211.json&sa=D&ust=1584094197112000)

1. Saving Exchange Rates into Database.
    * All Requested Exchange Rates to be saved into Database so that next time user request Exchange Rates for already saved date into DB, chatbot will return rates from DB, otherwise from API.

1.  Knex migration for creating table where Exchange Rates will be saved.

### Front-End Features:
1.  Show Chatbot Users Metrics in Botpress Admin Panel:
    * Conversation count
    * Exchange Calculator Usage count

## Technology Stack
* Botpress v10.x
* Getting Started Guide: [https://botpress.io/docs/10.50/getting_started](https://www.google.com/url?q=https://botpress.io/docs/10.50/getting_started&sa=D&ust=1584094197114000)
* How-tos and examples: [https://botpress.io/docs/10.34/recipes](https://www.google.com/url?q=https://botpress.io/docs/10.34/recipes&sa=D&ust=1584094197114000)
* API Reference: [https://botpress.io/docs/10.34/reference](https://www.google.com/url?q=https://botpress.io/docs/10.34/reference&sa=D&ust=1584094197114000)
* Language: NodeJS
* DataBase: Postgresql
* Platform: Docker
