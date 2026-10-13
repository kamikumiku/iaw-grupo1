## 1. Su sitio en Apache
VirtualHost en `conf/soporte.conf`, raíz en `/var/www/soporte`.

$ curl -H "Host: soporte.abdel.local" http://localhost/
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="utf-8">
    <title>Soporte · Abdel</title>
</head>
<body>
    <h1>Soporte</h1>
    <p>Departamento de Soporte de Abdel.</p>
</body>
</html>

$ sudo apache2ctl -S | grep soporte
         port 80 namevhost soporte.abdel.local (/etc/apache2/sites-enabled/soporte.conf:1)
