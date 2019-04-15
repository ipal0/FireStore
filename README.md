## Google Cloud FireStore Database Utilities for following functions:
* To List All Collections
* To Backup Collections 
* To Restore Collection
* To Convert CSV File to Collection

## Installation:
* Download the FireStore.py

## Usage Examples:

### Initialize the FireStore Database
import FireStore
db = FireStore.db()

### Backup:
* db.backup('collection_name') ....for single collection
* 	This will create a collection_name.json file as backup
* db.backup('col1', 'col2', 'col3') ...for multiple collections
* 	This will create multiple jsons files - col1.json to col3.json as backup
* db.backup(All=True) 
*	This will create json backup files for all collections in the database.

### Restore:
* db.restore('collection_name.json')
* This will create a collection with name "collection_name"

### Convert from CSV:
* db.csv2collection(CSV_FileName)
* This will convert a CSV File to Collection.
* Optional keyword argument name can be supplied to assign document name. 

### To List all Collections:
* db.list()
