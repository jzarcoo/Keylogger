# Keylogger

> Sistema que registra pulsaciones en el teclado.

**IBM Selectric II**

![IBM Selectric II](https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/IBM_Selectric_I_%284%29.jpg/280px-IBM_Selectric_I_%284%29.jpg)


---

## Organización

- `manifest.json` La configuración y metadatos de la extensión.
- `background.js` El script
- `options.js` y `options.xhtml` Menú para configurar el servidor de datos

## Servidor

`about:debugging`

```py
python3 -m http.server
> Serving HTTP on 0.0.0.0 port 8000 (http://0.0.0.0:8000/) ...
```

`http://localhost:8000/`

Crea llave pública y privada.

```sh
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout key.pem -out cert.pem
```

Agregar IP con dominio

```sh
sudo nano /etc/hosts
```

Añadir excepción

`about:preferences#privacy`