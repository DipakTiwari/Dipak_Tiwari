Project Setup and Execution Guide
----------------------------------------
1. Run Migrations and Seeders

	Create database with on your server and add database credentials in .env file:

	File Path:dipak_tiwari\.env

	Example:
	DB_CONNECTION=mysql
	DB_HOST=127.0.0.1
	DB_PORT=3306
	DB_DATABASE=dipak_tiwari
	DB_USERNAME=root
	DB_PASSWORD=
	
	After that run this command
	php artisan migrate
	
2. Start the Queue Worker

	In a separate terminal window, run the following command to start the queue worker:
	
	php artisan queue:work
	
3. Start the Development Server

	Once all the above steps are completed, start the development server using:
	
	php artisan serve
	
4. Run Tests

	For this you have to create and update .env file with your testing database credentials.
	
	Example:
	DB_CONNECTION=mysql
	DB_HOST=127.0.0.1
	DB_PORT=3306
	DB_DATABASE=dipak_tiwari_test
	DB_USERNAME=root
	DB_PASSWORD=
	
	To verify that everything is working as expected, run the tests using:
	
	php artisan test
	
