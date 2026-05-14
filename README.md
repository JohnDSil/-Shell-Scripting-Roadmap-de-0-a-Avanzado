# 🖥️ Shell Scripting Roadmap: de 0 a Avanzado

> **Aprende a dominar la terminal en Linux y Windows al mismo tiempo.**  
> Cada concepto se enseña en paralelo: primero en **Bash** (Linux/macOS), luego en **PowerShell** (Windows). Misma idea, dos lenguajes.

---

## 🎯 ¿Para quién es este repositorio?

Para estudiantes que:

- **Nunca han abierto una terminal** — empezamos desde cero absoluto
- Vienen del [Scripts Roadmap de Python](https://github.com/tu-usuario/scripts-roadmap) y quieren dar el salto a la terminal
- Quieren aprender administración de sistemas, automatización o DevOps
- Necesitan trabajar en entornos Linux Y Windows

No necesitas saber programar. Solo necesitas curiosidad y una terminal.

---

## 💡 La idea central: mismo concepto, dos lenguajes

Cada script de este repositorio resuelve **el mismo problema** en ambos sistemas:

```
📁 01-terminal-basica/
   ├── bash/
   │   └── 01_navegacion.sh      ← Navegar carpetas en Linux
   └── powershell/
       └── 01_navegacion.ps1     ← Navegar carpetas en Windows
```

Así aprenderás que los conceptos son universales: variables, bucles, condiciones, pipes... Solo cambia la sintaxis. Cuando domines uno, el otro te resultará familiar.

---

## 🗺️ Hoja de ruta

| Nivel | Carpeta | Contenido | Bash | PowerShell |
|-------|---------|-----------|------|-----------|
| 1 | [`01-terminal-basica`](./01-terminal-basica/) | Navegar, archivos, variables, primer script | `.sh` | `.ps1` |
| 2 | [`02-control-flujo`](./02-control-flujo/) | if/else, bucles for y while, case/switch | `.sh` | `.ps1` |
| 3 | [`03-texto-y-datos`](./03-texto-y-datos/) | grep, sed, awk, pipes, filtros | `.sh` | `.ps1` |
| 4 | [`04-sistema`](./04-sistema/) | Procesos, usuarios, red, tareas programadas | `.sh` | `.ps1` |
| 5 | [`05-automatizacion`](./05-automatizacion/) | Backups, logs, monitorización, alertas | `.sh` | `.ps1` |
| 6 | [`06-proyectos`](./06-proyectos/) | Scripts reales completos en ambos sistemas | `.sh` | `.ps1` |

---

## 🚀 Cómo usar este repositorio

### Paso 1 — Abre una terminal

**En Linux / macOS:**
```
Busca "Terminal" en tus aplicaciones
O pulsa: Ctrl + Alt + T  (en la mayoría de distros Linux)
```

**En Windows:**
```
Pulsa: Windows + X → "Windows PowerShell"
O busca "PowerShell" en el menú de inicio
O busca "Terminal de Windows" si la tienes instalada
```

### Paso 2 — Clona el repositorio

```bash
# En Bash (Linux/macOS):
git clone https://github.com/tu-usuario/shell-scripting-roadmap.git
cd shell-scripting-roadmap

# En PowerShell (Windows):
git clone https://github.com/tu-usuario/shell-scripting-roadmap.git
Set-Location shell-scripting-roadmap
```

### Paso 3 — Da permisos de ejecución (solo Linux/macOS)

```bash
chmod +x 01-terminal-basica/bash/*.sh
```

### Paso 4 — Ejecuta tu primer script

```bash
# En Bash:
bash 01-terminal-basica/bash/01_navegacion.sh

# En PowerShell:
.\01-terminal-basica\powershell\01_navegacion.ps1
```

### Paso 5 — Sigue el orden

Lee el `README.md` de cada nivel antes de ejecutar los scripts. **No saltes niveles** — cada uno depende del anterior.

---

## 📁 Estructura completa del repositorio

```
shell-scripting-roadmap/
│
├── README.md                          ← Estás aquí
│
├── 01-terminal-basica/
│   ├── README.md
│   ├── bash/
│   │   ├── 01_navegacion.sh           # cd, ls, pwd, mkdir, rm
│   │   ├── 02_archivos.sh             # touch, cp, mv, cat, echo
│   │   ├── 03_variables.sh            # Variables y strings
│   │   ├── 04_permisos.sh             # chmod, chown, ls -la
│   │   └── 05_primer_script.sh        # Shebang, ejecución, argumentos
│   ├── powershell/
│   │   ├── 01_navegacion.ps1          # Set-Location, Get-ChildItem
│   │   ├── 02_archivos.ps1            # New-Item, Copy-Item, Move-Item
│   │   ├── 03_variables.ps1           # $variables y strings
│   │   ├── 04_permisos.ps1            # Get-Acl, icacls
│   │   └── 05_primer_script.ps1       # Parámetros, ejecución
│   └── retos/
│       └── retos.md
│
├── 02-control-flujo/
│   ├── README.md
│   ├── bash/
│   │   ├── 01_if_else.sh              # Condicionales y comparaciones
│   │   ├── 02_bucle_for.sh            # for clásico y for-in
│   │   ├── 03_bucle_while.sh          # while y until
│   │   ├── 04_case.sh                 # case (equivalente a switch)
│   │   └── 05_menu_interactivo.sh     # Proyecto: menú de administración
│   ├── powershell/
│   │   ├── 01_if_else.ps1
│   │   ├── 02_foreach.ps1
│   │   ├── 03_while.ps1
│   │   ├── 04_switch.ps1
│   │   └── 05_menu_interactivo.ps1
│   └── retos/
│       └── retos.md
│
├── 03-texto-y-datos/
│   ├── README.md
│   ├── bash/
│   │   ├── 01_grep_buscar.sh          # grep, egrep, patrones
│   │   ├── 02_sed_reemplazar.sh       # sed para editar texto en masa
│   │   ├── 03_awk_procesar.sh         # awk para columnas y cálculos
│   │   ├── 04_pipes_filtros.sh        # |, sort, uniq, cut, wc
│   │   └── 05_procesar_csv.sh         # Proyecto: analizar un CSV real
│   ├── powershell/
│   │   ├── 01_select_string.ps1       # Select-String (como grep)
│   │   ├── 02_reemplazar_texto.ps1    # -replace, regex
│   │   ├── 03_objetos_filtros.ps1     # Where-Object, Select-Object
│   │   ├── 04_pipes_powershell.ps1    # Pipeline de objetos
│   │   └── 05_procesar_csv.ps1        # Import-Csv, Export-Csv
│   └── retos/
│       └── retos.md
│
├── 04-sistema/
│   ├── README.md
│   ├── bash/
│   │   ├── 01_procesos.sh             # ps, top, kill, jobs
│   │   ├── 02_usuarios.sh             # whoami, useradd, groups, sudo
│   │   ├── 03_red.sh                  # ping, netstat, curl, wget
│   │   ├── 04_cron.sh                 # crontab, tareas programadas
│   │   └── 05_info_sistema.sh         # Proyecto: informe del sistema
│   ├── powershell/
│   │   ├── 01_procesos.ps1            # Get-Process, Stop-Process
│   │   ├── 02_usuarios.ps1            # Get-LocalUser, net user
│   │   ├── 03_red.ps1                 # Test-Connection, Invoke-WebRequest
│   │   ├── 04_tareas_programadas.ps1  # Register-ScheduledTask
│   │   └── 05_info_sistema.ps1        # Proyecto: informe del sistema
│   └── retos/
│       └── retos.md
│
├── 05-automatizacion/
│   ├── README.md
│   ├── bash/
│   │   ├── 01_backups.sh              # rsync, tar, copias con fecha
│   │   ├── 02_logs_y_alertas.sh       # Rotar logs, alertas por email
│   │   ├── 03_monitorizacion.sh       # Monitorizar CPU, disco, red
│   │   ├── 04_despliegue.sh           # Script de deploy básico
│   │   └── 05_mantenimiento.sh        # Proyecto: script de mantenimiento
│   ├── powershell/
│   │   ├── 01_backups.ps1
│   │   ├── 02_logs_y_alertas.ps1
│   │   ├── 03_monitorizacion.ps1
│   │   ├── 04_despliegue.ps1
│   │   └── 05_mantenimiento.ps1
│   └── retos/
│       └── retos.md
│
└── 06-proyectos/
    ├── README.md
    ├── proyecto-backup-automatico/
    │   ├── backup.sh                  ← Versión Linux
    │   ├── backup.ps1                 ← Versión Windows
    │   └── README.md
    ├── proyecto-monitor-sistema/
    │   ├── monitor.sh
    │   ├── monitor.ps1
    │   └── README.md
    └── proyecto-instalador/
        ├── instalar.sh                ← Instala y configura un entorno
        ├── instalar.ps1
        └── README.md
```

---

## 🔤 Tabla de equivalencias rápida

Una referencia para cuando saltas entre sistemas:

| Acción | Bash (Linux) | PowerShell (Windows) |
|--------|-------------|---------------------|
| Listar archivos | `ls` | `Get-ChildItem` / `ls` |
| Cambiar carpeta | `cd carpeta` | `Set-Location carpeta` / `cd` |
| Carpeta actual | `pwd` | `Get-Location` / `pwd` |
| Crear carpeta | `mkdir nombre` | `New-Item -Type Directory` / `mkdir` |
| Crear archivo | `touch archivo.txt` | `New-Item archivo.txt` |
| Copiar | `cp origen destino` | `Copy-Item origen destino` |
| Mover | `mv origen destino` | `Move-Item origen destino` |
| Eliminar | `rm archivo` | `Remove-Item archivo` |
| Ver contenido | `cat archivo` | `Get-Content archivo` |
| Buscar texto | `grep "texto" archivo` | `Select-String "texto" archivo` |
| Variable | `nombre="valor"` | `$nombre = "valor"` |
| Imprimir | `echo "texto"` | `Write-Host "texto"` |
| Ejecutar script | `bash script.sh` | `.\script.ps1` |
| Ayuda de comando | `man ls` | `Get-Help Get-ChildItem` |
| Permisos | `chmod +x archivo` | `Set-ExecutionPolicy` |
| Procesos | `ps aux` | `Get-Process` |
| Matar proceso | `kill PID` | `Stop-Process -Id PID` |
| Red | `ping host` | `Test-Connection host` |
| Descargar | `curl -O url` | `Invoke-WebRequest url` |
| Tarea programada | `crontab -e` | `Register-ScheduledTask` |

---

## ⚙️ Requisitos

### Para Bash (Linux / macOS)
- Cualquier distribución Linux moderna (Ubuntu, Fedora, Arch...)
- macOS con Terminal o iTerm2
- En Windows: instala **WSL2** (Windows Subsystem for Linux) → [Guía oficial](https://learn.microsoft.com/es-es/windows/wsl/install)

### Para PowerShell (Windows)
- Windows 10 / 11 con PowerShell 5.1 (ya viene instalado)
- Recomendado: **PowerShell 7** → [Descargar aquí](https://github.com/PowerShell/PowerShell/releases)
- Editor recomendado: [VS Code](https://code.visualstudio.com/) con la extensión PowerShell

### Para ambos (recomendado)
- **Git** → [git-scm.com](https://git-scm.com/)
- **VS Code** con extensiones: *Bash IDE* y *PowerShell*

---

## 🛡️ Antes de empezar: regla de oro

> ⚠️ **Los scripts de sistema son poderosos. Un error puede borrar archivos o romper configuraciones.**

Sigue siempre estas normas:

1. **Lee el script antes de ejecutarlo.** Siempre.
2. **Practica en una carpeta de pruebas**, nunca directamente en tus documentos importantes.
3. **Nunca ejecutes scripts de internet sin entenderlos.**
4. **En Linux:** evita usar `sudo` hasta que entiendas exactamente qué hace el comando.
5. **Haz backups** antes de scripts que modifican archivos en masa.

---

## 📚 Recursos adicionales

**Bash:**
- [The Linux Command Line (gratis online)](https://linuxcommand.org/tlcl.php)
- [Bash scripting cheatsheet](https://devhints.io/bash)
- `man bash` — el manual completo en tu propia terminal

**PowerShell:**
- [Documentación oficial Microsoft](https://learn.microsoft.com/es-es/powershell/)
- [PowerShell Gallery](https://www.powershellgallery.com/) — módulos de la comunidad
- `Get-Help about_*` — tutoriales integrados en PowerShell

**Ambos:**
- [ExplainShell](https://explainshell.com/) — pega un comando y te explica cada parte
- [ShellCheck](https://www.shellcheck.net/) — detecta errores en scripts Bash

---

## 🤝 Relación con el Python Roadmap

Este repositorio es el **compañero natural** del [Scripts Roadmap de Python](../scripts-roadmap/). Se complementan así:

| Python Roadmap | Shell Roadmap |
|---------------|--------------|
| Lógica y algoritmos | Administración del sistema |
| Manipular datos (CSV, JSON) | Manipular archivos y procesos |
| Automatización con librerías | Automatización nativa del SO |
| Portable (igual en todos los SO) | Nativo de cada sistema |

En la práctica profesional, **se usan juntos**: un script de shell lanza un script de Python, o Python genera un script de shell. Aprenderlos en paralelo es la mejor inversión.

---

*Hecho con ❤️ para estudiantes que quieren dominar la terminal desde cero.*
