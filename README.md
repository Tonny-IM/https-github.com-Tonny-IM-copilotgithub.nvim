# https-github.com-Tonny-IM-copilotgithub.nvim
# copilotgithub.nvim

Automatiza la creación de repositorios de GitHub desde Neovim en Termux.

## Instalación

1. **Requisitos previos:**  
   Instala dependencias y configura la autenticación:
   ```bash
   pkg install git gh neovim nodejs
   gh auth login
   gh config set git_protocol ssh
   gh auth setup-git
   ```

2. **Instala el plugin** (ejemplo usando [vim-plug](https://github.com/junegunn/vim-plug)):
   ```vim
   Plug 'Tonny-im/copilotgithub.nvim'
   ```

3. **Carga la configuración mínima:**
   ```vim
   lua require("copilotgithub").setup()
   ```

## Uso

1. Abre Neovim en el directorio de tu proyecto.
2. Ejecuta:
   ```
   :CopilotGitHubCreateRepo
   ```
3. Sigue los prompts interactivos.

## Características

- 🚀 Crea repositorios públicos en GitHub
- 🤖 Automatiza `git init`, commit inicial, y push
- 🔐 Usa autenticación segura via GitHub CLI
- 🖥 Muestra progreso en terminal flotante
- 📦 Plugin estándar de Neovim

## Mejoras futuras

- Soporte para repos privados
- Selección de licencia
- Manejo de errores detallado
- Integración Copilot API
- Templates de repositorio

## Notas

- Requiere configuración previa de `gh`
- Necesita conexión a internet activa
- Ejecuta dentro de un directorio existente
- Asegúrate de tener permisos de escritura en GitHub

---
