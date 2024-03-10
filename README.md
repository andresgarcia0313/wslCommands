Listado de comandos para Windows Subsystem for Linux (WSL):

- Lista distribuciones WSL disponibles para instalación. ```wsl --list --online```
- Lista distribuciones WSL ```wsl -l -v```
- Cierra la instancia de Ubuntu en ejecución. ```wsl --terminate Ubuntu```
- Cierra las instancians en ejecución. ```wsl --shutdown```
- Elimina una distribución WSL. ```wsl --unregister Ubuntu```
- Muestra comandos de WSL en historial. ```Get-Content (Get-PSReadLineOption).HistorySavePath | Where-Object { $_ -like "*wsl*" }```
- Los WSL deben consumir solamente la mitad de ram fisica y procesador
Abre archivo de configuración de WSL en Notepad. ```notepad .wslconfig```
    ```
    [wsl2]
    memory=3GB
    processors=4
    swap=10GB
    ```
- Abre la carpeta de las distribuciones WSL en Explorador de archivos
   ```explorer \\wsl$```