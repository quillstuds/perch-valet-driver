# perch-valet-driver
A custom driver for Perch CMS to run properly in the Laravel Valet development environment.

Perch CMS seems to run fine in Laravel Valet, except that Perch can't validate your license on a Valet domain. This driver fixes that by setting `$_SERVER['SERVER_NAME']` correctly.

To install add this file to the '/Users/_your-user-name_/.valet/Drivers' folder.

If you're running an older version of Perch you will need to upgrade for this to work - Perch 2.8 wouldn't work so I assume anything lower will also need to be upgraded.

More info on Valet custom drivers can be found at https://laravel.com/docs/5.4/valet#custom-valet-drivers

This file is based on Basic Valet Driver, which can be found at https://github.com/laravel/valet/blob/master/cli/drivers/BasicValetDriver.php
