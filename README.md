1️⃣ Repo strukturasi
common_models/ \n
├─ common_models/ \n
│  ├─ __init__.py \n
│  ├─ models.py \n
│  └─ apps.py \n
├─ pyproject.toml \n
└─ README.md \n

2️⃣ apps.py \n
from django.apps import AppConfig \n

class CommonModelsConfig(AppConfig): \n
    name = 'common_models' \n

3️⃣ pyproject.toml \n
[build-system] \n
requires = ["setuptools"] \n
build-backend = "setuptools.build_meta" \n

[project] \n
name = "common-models" \n
version = "0.1.0" \n
dependencies = ["Django>=3.2"] \n

4️⃣ GitHub’ga push qil \n
5️⃣ Django projectda o‘rnatish \n
pip install git+https://github.com/you/common_models.git \n

6️⃣ INSTALLED_APPS \n
INSTALLED_APPS = [ \n
    ... \n
    'common_models', \n
]
 \n
7️⃣ Migratsiya \n
python manage.py makemigrations common_models \n
python manage.py migrate \n

\n
✅ Natija: \n

Bitta models.py → ko‘p project \n

Git bilan versiya nazorati \n

Eng professional yechim \n

Xohlasang PyPI’ga chiqarish yoki versioning ham qilib beraman. \n
