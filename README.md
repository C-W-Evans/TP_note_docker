Briève explication sur comment configurer et utiliser le stack docker

Prérequis
Docker et Docker Compose

Setup
Clone the Repository:
bash
Copier le code
git clone <repository_url>
cd <repository_name>
Build and Launch:
bash
Copier le code
docker-compose up --build
Access Services:
Frontend: http://localhost
PhpMyAdmin: http://localhost:8082
TensorFlow: http://localhost:8501/v1/models/placeholder_model
Services
Service	Port	Description
Frontend	80	Angular App
Backend	5000	Flask API
MySQL	3306	Database
PhpMyAdmin	8082	DB Management
TensorFlow	8501	Model Serving
Notes
Modify database credentials in docker-compose.yml if needed.
Place TensorFlow models in ./tensorflow_models.
