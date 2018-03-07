# Django 2.0 startproject template with bootstrap 4.0

Just updates the following:

### Set templates DIR

```
TEMPLATES = [  
    {  
        'BACKEND': 'django.template.backends.django.DjangoTemplates',
        'DIRS': [os.path.join(BASE_DIR, 'templates')],
        'APP_DIRS': True,
        'OPTIONS': {
            'context_processors': [
                'django.template.context_processors.debug',
                'django.template.context_processors.request',
                'django.contrib.auth.context_processors.auth',
                'django.contrib.messages.context_processors.messages',
            ],
        },
    },
]
```

### Set timezone to EST
```
TIME_ZONE = 'EST'
```

### Add static files and media
```
STATICFILES_DIRS = [
    os.path.join(BASE_DIR, 'static')
]

STATIC_URL = '/static/'
STATIC_ROOT = os.path.join(BASE_DIR, 'assets')

MEDIA_ROOT = os.path.join(BASE_DIR, 'media')

MEDIA_URL = '/media/'
```

### Create a views.py in project folder
### Create a static folder in root
### Create a media folder in root
### Create a templates folder in root
```
templates
└── base
    ├── footer.html
    ├── footer_js.html
    └── header.html
```


