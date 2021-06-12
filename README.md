# CarTrack Interview Test [Kalai]

REST Api project without framework dependencies.

##Installation
- Pull the repository to your local.
- Default configuration is using database from AWS.  

## Usage
I've used `cars` table from provided details.

### Routes as follow
Assuming `cartrack.test` is the virtual domain.

METHOD  | Route | Content Body | Description
------------- | -------------| -------------| -------------
GET     | `cartrack.test`| -| - to list all record
GET     | `cartrack.test/{id}`| -| - to list record by id
POST    | `cartrack.test`| {"name": "Hilux","type": "Sedan","brand": "Toyota","year": "2020"}| - to create new record
PUT     | `cartrack.test/{id}`| {"name": "Hilux","type": "Sedan","brand": "Toyota","year": "2020"}| - to update old record with given id
DELETE  | `cartrack.test/{id}`| -| - to delete record by id

### Validation

- [x] Accessing `GET` Method with invalid `id`
- [x] Accessing `PUT` Method with invalid `id`
- [x] Accessing `DELETE` Method with invalid `id`
- [x] Accessing `POST` Method with invalid post data
- [x] Accessing `PUT` Method with invalid post data

