# Example Unit testing with laravel



## Requirements
- PHP
- Composer
- Docker
- Laravel Sail
- Node.js and npm (if applicable)

## Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd <project-directory>
   ```

2. **Install dependencies**:
   Run the following command to install PHP dependencies using Composer:
   ```bash
   composer install
   ```

3. **Set up environment variables**:
   Copy the `.env.example` file to `.env` and configure it as needed:
   ```bash
   cp .env.example .env
   ```

4. **Start Docker containers**:
   Ensure Docker is running, then start the containers using Laravel Sail:
   ```bash
   ./vendor/bin/sail up -d
   ```

5. **Run database migrations**:
   Execute the following command to set up the database:
   ```bash
   ./vendor/bin/sail artisan migrate
   ```

6. **Install front-end dependencies** (if applicable):
   ```bash
   npm install
   npm run dev
   ```

## Running Tests
To run the test suite, use the following command:
```bash
./vendor/bin/sail artisan test
```

## Usage
Access the application in your browser at:
```
http://localhost
```

## Additional Commands
- **Stop Docker containers**:
  ```bash
  ./vendor/bin/sail down
  ```

- **Rebuild containers** (if needed):
  ```bash
  ./vendor/bin/sail build
  ```

```
