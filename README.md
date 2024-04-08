# Number Guessing Database Project

This project is a simple number guessing game implemented using a PostgreSQL database. It allows players to guess a randomly generated number and records their guesses in the database. Players can see their game history and statistics, such as the number of games played and their best game.

## Files

- **number_guessing.sh**: Bash script to interact with the database, allowing players to play the number guessing game and recording game data.
- **number_guess.sql**: SQL file containing the database schema and initial setup.
- **README.md**: This file, providing an overview of the project.

## Usage

1. **Setup Database**: Run the `number_guess.sql` script to create the necessary tables and schema in your PostgreSQL database.
   
   ```bash
   psql -U <username> -d <database_name> -a -f number_guess.sql
2. ## Run Game

Execute the `number_guessing.sh` script to play the number guessing game and interact with the database.

```bash
bash number_guessing.sh
```
## Database Schema

The database consists of two tables:

- **players**: Stores player information, including their unique ID and username.
- **games**: Records each game played, including the user ID, the secret number, and the number of guesses made.

### Dependencies

- PostgreSQL
## License

This project is licensed under the MIT License.
