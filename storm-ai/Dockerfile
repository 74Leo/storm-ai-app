FROM python:3.11

WORKDIR /app

# Installer les dépendances
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copier les fichiers du projet
COPY . .

# Exposer le port pour l'accès web
EXPOSE 8000

# Lancer STORM AI
CMD ["streamlit", "run", "app.py", "--server.port=8000", "--server.address=0.0.0.0"]
