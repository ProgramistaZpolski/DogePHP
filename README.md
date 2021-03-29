# DogePHP
PHP Wrapper around the DogeHouse/DogeGarden API

Stuff left to be added: Ability to connect to a room

## Usage
```php
include_once "Master.php";

use ProgramistaZpolski\DogePHP\Doge;

Doge::info(); // Get info about the API - https://api.dogehouse.xyz/v1/
Doge::bots(); // Get the list of bots - https://api.dogehouse.xyz/v1/bots
Doge::stats(); // Get some statistics - https://api.dogehouse.xyz/v1/statistics
Doge::rooms("popular"); // Get popular rooms - https://api.dogehouse.xyz/v1/popularRooms
Doge::rooms("scheduled"); // Get scheduled rooms - https://api.dogehouse.xyz/v1/scheduledRooms
```

### Speed
API Requests Speed for a 10kb/s upload, 40kb/s download internet connection:
```php
Doge::info(); // ~15s
Doge::stats(); // ~20s
Doge::bots(); // ~260s
Doge::rooms("popular"); // ~5s
Doge::rooms("scheduled"); // ~7s
```
