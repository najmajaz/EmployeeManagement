# EmployeeManagement
.env file


       DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=employee
DB_USERNAME=root
DB_PASSWORD=




     Migrations create table

      Schema::create('employee_details', function (Blueprint $table) {
            $table->id(); // Auto-incrementing ID
            $table->string('first_name');
            $table->string('last_name');
            $table->string('email')->unique(); // Unique email field
            $table->string('phone')->nullable(); // Phone number (nullable)
            $table->string('department')->nullable(); // Department (nullable)
            $table->decimal('salary', 10, 2); // Salary with two decimal places
            $table->timestamps();

            });




     
