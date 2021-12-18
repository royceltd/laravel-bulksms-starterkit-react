### Laravel bulk sms starter kit

This starter kit runs on Laravel V8. It comes with Authentication (Login and registration) powered by laravel Breeza + Inertial React.

Happy hacking!!!

support info@roycetechnologies.co.ke Whatsapp/call 0713727937

#### installation

-   Clone this repo

###### Copy paste the following commands to set up

```
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
```

-   Generate API key from [Royce Bulk SMS]('https://bulksms.roycetechnologies.co.ke') and paste in the .env

```
API_KEY=apikey
SENDER_ID=RoyceLTD

```

-   run `php artisan serve`
-   visit [http://localhost:8000/bulksms]('http://localhost:8000/bulksms') to start sending Messages

###### To send from a controller import RoyceBulkSMS facade:

```
use RoyceLtd\LaravelBulkSMS\Facades\RoyceBulkSMS;

        $phone = "071234567";
        $message = "Hello world";

        RoyceBulkSMS::sendSMS($phone, $message);

```
