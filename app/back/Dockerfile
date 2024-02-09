# Utiliser une image Python comme base
FROM python:3.8

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier le fichier des dépendances et installer les dépendances
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copier le reste du code de l'application dans le conteneur
COPY . .

# Définir la commande pour démarrer l'application Flask
CMD ["python3", "-m", "flask", "run", "--host=0.0.0.0"]
