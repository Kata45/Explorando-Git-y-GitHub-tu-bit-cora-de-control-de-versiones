![Git Logo](https://habrastorage.org/getpro/habr/upload_files/3b6/487/9f7/3b64879f799e0181dec88e8fa4330c2e.png)

---

<div align="center">

<h1>🔶 Git en Acción</h1>

> ## 👩🏻‍💻*Kata*
> **Objetivo:** El presente informe tiene como objetivo recopilar los fundamentos clave sobre **Git** y **GitHub**, dos herramientas esenciales en el desarrollo de software moderno. Además, se incluyen reflexiones personales acerca de su importancia en el trabajo colaborativo y el control de versiones, así como un ejercicio práctico que demuestra la aplicación de los conceptos aprendidos.

</div>

---

<div align="center">
<h2>🔴 GIT</h2>
</div>

**Definición**

Es un sistema de control de versiones distribuido.  
Permite llevar un historial completo de los cambios de un proyecto y colaborar con otros sin perder información.

**Historia**

Antes de Git, los desarrolladores usaban herramientas como CVS y Subversion (SVN) para controlar versiones de código.  
Sin embargo, estos sistemas eran lentos y dependían de un servidor central.

En **2005**, el creador de Linux, **Linus Torvalds**, desarrolló **Git** para gestionar el código del núcleo (kernel) de Linux.  
Su objetivo era crear una herramienta:

- Rápida  
- Segura  
- Distribuida (sin depender de un servidor central)

Git permite que **cada desarrollador tenga una copia completa del repositorio**, lo que hace posible trabajar sin conexión y fusionar cambios fácilmente.

 **Año de creación:** 2005  
 **Creador:** Linus Torvalds  
 **Propósito:** Controlar versiones de software de manera eficiente y descentralizada  

**Objetivos**

- Guardar versiones de tus archivos.  
- Retroceder a versiones anteriores.  
- Trabajar en equipo sin sobrescribir cambios.  
- Llevar un registro exacto de quién, cuándo y qué se modificó.

>  *Git cambió la forma en que los programadores trabajan en equipo, marcando el inicio del desarrollo colaborativo moderno.*

---

<div align="center">
<h2>🟥 Instalación de Git</h2>
</div>

A continuación, se muestran los pasos para instalar **Git** en los diferentes sistemas operativos.

| Sistema Operativo | Instrucciones                                                                                         | Verificación                                           |
|-------------------|-------------------------------------------------------------------------------------------------------|--------------------------------------------------------|
| **Windows**       | 1. Ve a [Git para Windows](https://git-scm.com/download/win).<br>2. Ejecuta el instalador y sigue las instrucciones. <br>3. Deja las opciones por defecto. | Abre **Git Bash** y escribe: <br>`git --version`        |
| **macOS**         | 1. Si tienes **Homebrew** instalado, usa el siguiente comando: <br>`brew install git`.<br>2. Si no, descarga el instalador desde [Git para Mac](https://git-scm.com/download/mac). | Abre la terminal y escribe: <br>`git --version`         |
| **Linux (Debian/Ubuntu)** | 1. Ejecuta el siguiente comando en la terminal: <br>`sudo apt-get install git`.<br>2. Si usas otra distribución, usa el gestor de paquetes correspondiente. | Escribe en la terminal: <br>`git --version`            |
| **Linux (Fedora)** | 1. Usa el siguiente comando en la terminal: <br>`sudo dnf install git`. | Escribe en la terminal: <br>`git --version`            |

---

<div align="center">
<h1>Evidencias de Instalación</h1>
</div>

Se mostrará el paso a paso realizado en la instalación y configuración de Git:

### 1️⃣ Inicializar un repositorio local
```bash
git --version
```

---

<div align="center">
<h2>📌 Principales comandos de Git</h2>
</div>

| Comando | Descripción |
|----------|-------------|
| `git init` | Crea un nuevo repositorio local de Git. |
| `git status` | Muestra el estado actual de los archivos (modificados, nuevos, sin seguimiento). |
| `git add <archivo>` | Añade archivos al área de preparación (staging). |
| `git commit -m "mensaje"` | Guarda los cambios localmente con un mensaje descriptivo. |
| `git log` | Muestra el historial de commits realizados. |
| `git branch` | Muestra o crea nuevas ramas de trabajo. |
| `git checkout <rama>` | Cambia entre ramas del proyecto. |
| `git merge <rama>` | Fusiona los cambios de una rama con otra. |
| `git push` | Envía los commits locales al repositorio remoto. |
| `git pull` | Descarga los cambios desde el repositorio remoto. |
| `git clone <url>` | Copia un repositorio remoto a tu computadora. |

>  *Git trabaja localmente: todo el historial y las versiones se guardan en tu equipo.*

---

![Git Logo](https://i0.wp.com/puresourcecode.com/wp-content/uploads/2022/11/github-wallpaper-scaled.jpeg?fit=2560%2C1440&ssl=1)

<div align="center">
<h1>🐈‍⬛ Github</h1>
</div>

**GitHub** es una plataforma en la nube donde los desarrolladores almacenan y comparten proyectos que usan Git.  
Funciona como una red social para programadores: puedes seguir proyectos, colaborar en código y contribuir a otros repositorios.

**Historia Github**

Aunque Git solucionaba el control de versiones, no existía una forma sencilla de compartir proyectos por internet.  
Por eso, en **2008**, los desarrolladores **Tom Preston-Werner**, **Chris Wanstrath**, **PJ Hyett** y **Scott Chacon** crearon **GitHub**, una plataforma web basada en Git.

GitHub permitió:

- Subir repositorios a la nube.  
- Colaborar con otros mediante *pull requests* y *issues*.  
- Hacer proyectos públicos u organizacionales.  
- Contribuir fácilmente a proyectos *open source*.

En **2018**, **Microsoft** adquirió GitHub por **7.5 mil millones de dólares**, impulsando aún más su expansión.

🔹 **Año de creación:** 2008  
🔹 **Fundadores:** Tom Preston-Werner, Chris Wanstrath, PJ Hyett y Scott Chacon  
🔹 **Propiedad actual:** Microsoft  

**Objetivos**

- Crear y alojar repositorios en línea.  
- Trabajar con otros desarrolladores.  
- Hacer control de versiones de manera visual.  
- Publicar proyectos y portafolios.

> *GitHub convirtió Git en una herramienta accesible, social y colaborativa.*

---

<div align="center">
<h1>Diferencias</h1>
<h1>🔶 Git y Github 🐈‍⬛</h1>
</div>

| Característica | Git | GitHub |
|-----------------|-----|--------|
| Creación | 2005 | 2008 |
| Creador | Linus Torvalds | Tom Preston-Werner y equipo |
| Tipo de herramienta | Sistema de control de versiones | Plataforma en la nube |
| Uso principal | Control local del historial de versiones | Colaboración y publicación de proyectos |
| Necesita internet | No | Sí |
| Comando ejemplo | `git commit -m "mensaje"` | `git push origin main` |

> 💡 *Git gestiona el código, GitHub conecta personas.*

---

<div align="center">
<h1>Usar Juntos</h1>
<h1>🔶 Git y Github 🐈‍⬛</h1>
</div>

A continuación, el flujo de trabajo básico entre tu computadora (Git) y la nube (GitHub):

### 1️⃣ Inicializar un repositorio local
```bash
git init
```
