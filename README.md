Briève explication sur comment configurer et utiliser le stack docker

- Prérequis
Docker et Docker Compose

- Copier le code
git clone https://github.com/C-W-Evans/TP_note_docker
cd TP_note_docker

- Build et demarre
docker-compose up --build

- Accède aux services:
Frontend: http://localhost:4200/
PhpMyAdmin: http://localhost:8082
TensorFlow: http://localhost:8501/v1/models/placeholder_model

Mettez votre model TensorFlow dans le dossier ./tensorflow_models et enlevez les commentaires du la partie "# depends_on:
    #   - tensorflow" dans le Dockerfile du backend.
