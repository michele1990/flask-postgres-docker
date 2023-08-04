# Flask-Postgres-Docker Project

This project provides a simple setup for running a Flask application alongside a PostgreSQL database using Docker. The Flask application serves a web page that allows users to interact with the PostgreSQL database. Both the Flask application and PostgreSQL database are containerized using Docker and orchestrated with Docker Compose.

## Project Structure

The project is organized into the following directories:


flask-postgres-docker/
│
├── postgres/
│   ├── Dockerfile
│   └── init.sql (optional, for database initialization)
│
├── flask_app/
│   ├── templates/
│   │   └── index.html (HTML template for the web page)
│   ├── app.py (main application code)
│   ├── Dockerfile (Dockerfile for the Flask container)
│   └── requirements.txt (Python dependencies)
│
└── docker-compose.yml (Docker Compose file to orchestrate containers)


## Requirements

- Docker
- Docker Compose

## How to Run

1. Clone this repository to your local machine.

2. Navigate to the project directory:

   \`\`\`bash
   cd flask-postgres-docker
   \`\`\`

3. Build and start the containers using Docker Compose:

   \`\`\`bash
   docker-compose up --build
   \`\`\`

   To run the containers in detached mode, use:

   \`\`\`bash
   docker-compose up --build -d
   \`\`\`

4. Access the Flask application by opening your web browser and navigating to `http://localhost:5001`.

## Customization

- Modify the `app.py` file to change the Flask application's behavior.
- Edit the `Dockerfile` within the `flask_app` directory to adjust the Flask container setup.
- Modify the `init.sql` file within the `postgres` directory to customize the PostgreSQL database initialization.


## Contributions

Feel free to open an issue or submit a pull request if you have any improvements or suggestions.
