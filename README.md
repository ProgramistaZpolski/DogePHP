# DogePHP
PHP Wrapper around the DogeHouse/DogeGarden API

Stuff left to be added: Ability to connect to a room

## Usage
```php
include_once "Master.php";

use ProgramistaZpolski\DogePHP\Doge;

Doge::info(); // Get info about the API
Doge::bots(); // Get the list of bots
Doge::stats(); // Get some statistics
Doge::rooms("popular"); // Get popular rooms
Doge::rooms("scheduled"); // Get scheduled rooms
```
