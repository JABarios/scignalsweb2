Atacando la web

PING scignals.es (138.68.80.37) 56(84) bytes of data.
64 bytes from 138.68.80.37 (138.68.80.37): icmp_seq=1 ttl=49 time=46.4 ms
64 bytes from 138.68.80.37 (138.68.80.37): icmp_seq=2 ttl=49 time=45.2 ms
64 bytes from 138.68.80.37 (138.68.80.37): icmp_seq=3 ttl=49 time=47.9 ms


digital ocean
wordpress-512mb-fra1-01-scignals-com
juan --> jbh1501

github/signalsweb2


# 🧾 Configuración Apache para Sitio Multilingüe de Scignals


## 🌐 Dominios y Subdominios

| Dominio / Subdominio       | Idioma   | Carpeta en servidor                   | Método de despliegue  |
|----------------------------|----------|----------------------------------------|------------------------|
| `www.scignals.com`         | Inglés   | `/var/www/html/scignals_com`          | Hugo → `--language en` |
| `es.scignals.com`          | Español  | `/var/www/html/scignals_es`           | Hugo → `--language es` |
| `www.scignals.es`          | Español  | `/var/www/html/scignals_es`           | Hugo → `--language es` |

---

## 🏗️ Apache Virtual Hosts

Se han definido tres archivos de configuración en `/etc/apache2/sites-available/`, uno por dominio/subdominio:

### `scignals.conf`
- **ServerName:** `www.scignals.com`
- **DocumentRoot:** `/var/www/html/scignals_com`
- **Idioma:** Inglés
- **HTTPS:** Configurado con certificado SSL

### `scignals_es.conf`
- **ServerName:** `es.scignals.com`
- **DocumentRoot:** `/var/www/html/scignals_es`
- **Idioma:** Español
- **HTTPS:** Configurado con certificado SSL

### `scignals_punto_es.conf`
- **ServerName:** `www.scignals.es`
- **DocumentRoot:** `/var/www/html/scignals_es`
- **Idioma:** Español
- **HTTPS:** Configurado con certificado SSL

Todos los virtual hosts redirigen automáticamente desde HTTP (`:80`) a HTTPS (`:443`).

---

## 🔐 Seguridad SSL

Cada dominio utiliza certificados SSL individuales, gestionados mediante Let's Encrypt. Configuración típica:

```apache
SSLEngine on
SSLCertificateFile      /etc/letsencrypt/live/DOMINIO/fullchain.pem
SSLCertificateKeyFile   /etc/letsencrypt/live/DOMINIO/privkey.pem
```

Y redirección desde HTTP:

```apache
<VirtualHost *:80>
    ServerName www.scignals.com
    Redirect permanent / https://www.scignals.com/
</VirtualHost>
```

---

## ⚙️ Generación de Sitios con Hugo

Los sitios web se generan de forma estática usando Hugo, con estructura multilingüe.

```bash
# Sitio en inglés
hugo --language en --destination /var/www/html/scignals_com --baseURL="https://www.scignals.com"

# Sitio en español
hugo --language es --destination /var/www/html/scignals_es --baseURL="https://www.scignals.es"
```

---

## ✅ Comentarios Finales

- Configuración robusta y profesional.
- Cada idioma tiene su propio dominio o subdominio dedicado.
- HTTPS en todos los casos, con redirección desde HTTP.
- Hugo permite mantener el contenido actualizado y separado por idioma.
- El subdominio `es.scignals.com` podría redirigirse a `www.scignals.es` si se desea unificar tráfico.

---

