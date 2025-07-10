# demo

Este repositorio muestra cómo generar y configurar una llave SSH para conectarte con GitHub de forma segura.

---

## 🔑 Generar una nueva llave SSH

Sigue la documentación oficial de GitHub para generar una nueva llave SSH y añadirla al agente SSH:

👉 [Generar llave SSH y añadirla al SSH Agent](https://docs.github.com/es/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

---
## en caso de pedir permisos despues de eval
    chmod 400 ~/.ssh/Nombre_clave
---

## ⚙️ Configurar el archivo SSH (`~/.ssh/config`)

Edita (o crea si no existe) el archivo `~/.ssh/config` y agrega lo siguiente:

```ssh-config
Host *
	AddKeysToAgent yes
	# UseKeychain yes  # (Solo si usas macOS)
	IdentityFile ~/.ssh/Nombre_llave_privada
	


