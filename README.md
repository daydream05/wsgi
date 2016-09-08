# wsgi
wsgi for deploying web app

import os
import sys

path = '/home/ianparulan/AttendanceApp'
if path not in sys.path:
    sys.path.append(path)

os.environ['DJANGO_SETTINGS_MODULE'] = 'sigma.settings'

from django.core.wsgi import get_wsgi_application
application = get_wsgi_application()
