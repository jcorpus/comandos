Comandos Windows
----------------
**Procesos en ejecución, eliminarlos, puertos activos y más**

##### tasklist (procesos en ejecución)
`tasklist`

`netstat -oan` -o muestra el PID, a- las conexiones y n- las direcciones ip.

**Nombre de la aplicacion del proceso**

`tasklist /svc /FI "PID eq 234"` conocer el nombre de la aplicacion con PID 234.

`taskill /PID 234` para forzar el cierre de la aplicacion con PID 234.

`taskkill /F /IM notepad.exe` termina de manera forzada con los procesos.

