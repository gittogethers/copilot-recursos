# Configuración de GitHub Copilot en Diferentes IDEs

GitHub Copilot es compatible con varios entornos de desarrollo integrado (IDEs) populares. A continuación, te mostramos cómo configurarlo en cada uno de ellos:

## 1. Visual Studio Code

1. Abre Visual Studio Code.
2. Ve a la pestaña de **Extensiones** (Ctrl+Shift+X).
3. Busca "GitHub Copilot".
4. Haz clic en **Instalar**.
5. Una vez instalado, inicia sesión con tu cuenta de GitHub.

## 2. Visual Studio

1. Abre Visual Studio.
2. Ve a **Extensiones** > **Administrar Extensiones**.
3. Busca "GitHub Copilot".
4. Haz clic en **Descargar**.
5. Reinicia Visual Studio después de la instalación.
6. Inicia sesión con tu cuenta de GitHub cuando se te solicite.

## 3. JetBrains IDEs (IntelliJ IDEA, PyCharm, WebStorm, etc.)

1. Abre tu IDE de JetBrains.
2. Ve a **File** > **Settings** (en Windows/Linux) o **Preferences** (en macOS).
3. Navega a **Plugins**.
4. Busca "GitHub Copilot".
5. Haz clic en **Install**.
6. Reinicia el IDE después de la instalación.
7. Ve a **Tools** > **GitHub Copilot** > **Login to GitHub** para iniciar sesión.

## 4. Neovim

1. Asegúrate de tener Node.js instalado.
2. Instala el plugin de Copilot usando tu gestor de plugins preferido. Por ejemplo, con **vim-plug**:
   ```vim
   Plug 'github/copilot.vim'
   ```
3. Ejecuta `:PlugInstall` en Neovim.
4. Ejecuta `:Copilot setup` para iniciar sesión y autorizar Copilot.

## 5. Extensión del Navegador para GitHub.com

1. Ve a la [página de la extensión de GitHub Copilot](https://github.com/features/copilot).
2. Haz clic en **Install** para tu navegador (Chrome, Edge o Firefox).
3. Sigue las instrucciones para añadir la extensión a tu navegador.
4. Inicia sesión con tu cuenta de GitHub cuando se te solicite.

## Notas importantes:

- Asegúrate de tener una suscripción activa a GitHub Copilot.
- Para estudiantes, verifica si tienes acceso a través del [GitHub Student Developer Pack](https://github.com/gittogethers/copilot-recursos/blob/main/tutoriales/activacion-SDP.md).
- Mantén tu IDE y la extensión de Copilot actualizados para obtener las últimas características y mejoras.
- Si encuentras problemas, verifica tu conexión a internet y asegúrate de que tu firewall no esté bloqueando la conexión a los servidores de GitHub.
