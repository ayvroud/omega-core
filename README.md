# OMEGA SUITE - Système de Monitoring Crypto 📊

Stratégie d'accumulation BTC 2026-2035

## 📁 Structure du Projet

```
omega-suite/
├── .env.example          # Template des variables d'environnement
├── .gitignore           # Protection des fichiers sensibles
├── requirements.txt     # Dépendances Python
├── main.py             # Point d'entrée principal
└── src/
    ├── __init__.py     # Package Python
    └── db_setup.py     # Configuration et test Supabase
```

## 🚀 Installation et Configuration

### 1️⃣ Créer l'environnement virtuel

**Mac/Linux:**
```bash
# Créer le venv
python3 -m venv venv

# Activer le venv
source venv/bin/activate
```

**Windows:**
```bash
# Créer le venv
python -m venv venv

# Activer le venv
venv\Scripts\activate
```

### 2️⃣ Installer les dépendances

```bash
# Installer toutes les dépendances
pip install -r requirements.txt

# Vérifier l'installation
pip list
```

### 3️⃣ Configuration des variables d'environnement

```bash
# Copier le template
cp .env.example .env

# Éditer le fichier .env avec vos vraies credentials
nano .env  # ou vim, code, etc.
```

**⚠️ IMPORTANT:** Ne jamais commit le fichier `.env` sur GitHub!

### 4️⃣ Tester la connexion Supabase

```bash
# Exécuter le script de test
python src/db_setup.py
```

### 5️⃣ Lancer l'application

```bash
# Démarrer le système
python main.py
```

## 🔒 Sécurité

- ✅ Le fichier `.env` est dans `.gitignore`
- ✅ Ne jamais partager vos clés API
- ✅ Utiliser des clés API en lecture seule si possible
- ✅ Activer l'authentification 2FA sur Binance
- ✅ Restreindre les IPs autorisées dans Binance API settings

## 📦 Dépendances Principales

- `python-dotenv`: Gestion des variables d'environnement
- `ccxt`: Connexion aux exchanges crypto
- `supabase`: Base de données PostgreSQL
- `loguru`: Logging avancé
- `python-telegram-bot`: Notifications Telegram

## 🛠️ Prochaines Étapes

1. Remplir le fichier `.env` avec vos credentials
2. Créer les tables dans Supabase Dashboard
3. Implémenter la logique de récupération des prix BTC
4. Configurer les alertes et notifications
5. Développer la stratégie d'accumulation

## 📝 Notes

- Python 3.10+ requis
- Architecture modulaire pour faciliter l'évolution
- Logs automatiques dans le dossier `logs/`

---

*Développé avec ❤️ pour l'accumulation BTC*
