# Hito 1: Repositorio de prácticas y definición del proyecto

En este archivo se irán documentando todas las tareas asociadas al hito 1 de la asignatura.

## Configuración del repositorio

### Generación de una nueva clave SSH y adición de esta a GitHub

Para generar la clave SSH se ejecutó el siguiente comando:

```bash
ssh-keygen -t ed25519 -C "GitHub-feglez2000@gmail.com"
```

Una vez generada, esta se añadió a GitHub empleando los pasos mostrados en [Adding a new SSH key to your GitHub account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

### Configuración del nombre y del correo electrónico

Con tal de que el nombre y el correo electrónico aparezcan en los *commits*, se ejecutaron los siguientes comandos:

```bash
git config --global user.name "Felipe González López"
git config --global user.email "feglez2000@gmail.com"
```

### Personalización del perfil de GitHub

Para esto hice click sobre mi foto de perfil y accedí a *Settings* $\rightarrow$ *Public profile*. Dentro de este menú incluí los siguientes datos:

- ***Name:*** Felipe González López
- ***Profile photo:*** uploaded a photo of mine
- ***Company***: University of Granada
- ***Location:*** Granada, Granada, Spain

### Activación del segundo factor de autenticación (2FA)

Para activar el segundo factor de autenticación se siguieron los pasos mostrados en [Configuring two-factor authentication](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication).

En mi caso decidí emplear [DUO Mobile](https://duo.com/product/multi-factor-authentication-mfa/duo-mobile-app) como aplicación TOTP.