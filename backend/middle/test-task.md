## Test Task - Node REST API
### Description
- CRUD manipulations over the authors, books and publishers
https://en.wikipedia.org/wiki/Create,_read,_update_and_delete

#### Required endpoints
##### Authors
* Create author
* Get all authors
* Get one author
* Update author
* Remove author
* Get author books

##### Books
* Create book
* Get all books
* Get one book
* Update book
* Remove book
* Set book publisher
* Set book authors

##### Publishers
* Create publisher
* Get all publishers
* Get one publisher
* Update publisher
* Remove publisher
* Get publisher books

### Database structure
#### Author's fields
- first name
- last name
- birthday
- created at
- updated at
#### Book's fields
- title
- author
- publisher
- iban
- published at
- created at
- updated at
#### Publisher's fields
- title
- address
- created at
- updated at
### Task performance levels
1. Relations 
   - One Book can have many Authors
   - One Author can write many Books
   - One Book can be published by one Publisher
2. CRUD logic
2. OOP using Typescript
3. Linter + code formating
3. Validation
4. Tests
5. Swagger API Documentation
6. Postman Collection of API
### Required packages:
```
node
npm
express
jsonwebtoken
typescript
ts-node
sequelize
sequelize-typescript
dotenv
winston
socket.io
```
### Additional packages:
```
tsconfig-paths
tslint
tslint-config-prettier
prettier
nodemon
```
