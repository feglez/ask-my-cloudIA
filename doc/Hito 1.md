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

### Licencia empleada

Para este proyecto se ha decidido emplear una licencia MIT. Esta puede consultarse [aquí](https://github.com/feglez/ask-my-cloudIA/blob/main/LICENSE).

## Descripción del problema a resolver
Este proyecto trata de abordar un problema que tengo desde hace bastante tiempo. Soy una persona que está constantemente tratando de aprender cosas nuevas sobre todo tipo de temas como ciberseguridad, inteligencia artificial, filosofía, matemáticas, entre otros. Hasta ahora, cuando aprendía algo nuevo, unas veces tomaba apuntes a ordenador, otras a papel, y otras ni siquiera tomaba apuntes, lo que ha provocado que toda esa información sea poco accesible y esté descentralizada. A raíz de esto decidí empezar a utilizar Obsidian como gestor de conocimiento, y, si bien me está ayudando considerablemente, no ha resuelto el problema del todo.

### Posible solución
Para solucionar este problema se me ha ocurrido crear una infraestructura compuesta de un *Network Attached Storage (NAS)* y un *Large Language Model (LLM)*. La idea es que el NAS almacene y centralice todos mis apuntes, de forma que el LLM pueda aprender de ellos. De esta forma conseguiría tener una especie de "segundo cerebro digital" del que poder recuperar, de forma rápida y eficiente, la información que he ido aprendiendo a lo largo del tiempo.

En sus respuestas, este LLM podría, no solo responder a lo que se le pida, sino también indicar la nota de la que ha recuperado dicha información.

En caso de que esta solución llegase a funcionar, podría emplearla para almacenar no solo mi conocimiento, sino también el conocimiento de algún amigo, de forma que podría existir un LLM "fine-tuneado" para cada subconjunto de apuntes, y, luego, uno para el conjunto global, que haya sido entrenado con toda la información disponible en el NAS. 

La plataforma podría constar de dos tipos de usuarios:

- Usuario estándar: este tipo de usuario tendrá un espacio privado donde almacenar su información de forma segura, de forma que ningún otro usuario podría acceder a estos datos, ni acceder al LLM "fine-tuneado" con ellos (a menos que este le dé acceso).
- Usuario administrador: tendrá permisos para administrar los usuarios de la plataforma, así como para ajustar el espacio de almacenamiento disponible para cada uno de ellos.

### Justificación como proyecto en la nube
Las ventajas de desplegar este proyecto en la nube son claras:
- Acceso ubicuo a la información.
- Almacenaje centralizado de todos los apuntes.
- Disposición de una mayor capacidad de cómputo.
- Disponibilidad de la plataforma para otros usuarios.