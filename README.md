# Performance-k6-dashboard
Pasos
1- Instalar NodeJS en nuestra PC: https://nodejs.org/en
2- Instalar por por consola k6: https://grafana.com/docs/k6/latest/get-started/installation/
3- Instalar go (Mac): brew install go
4- Instalar xk6 a travez de go: go install go.k6.io/xk6/cmd/xk6@latest
5- Exportar las variables de entorno correspondientes para su SO: En mac: export PATH=$(go env GOPATH)/bin:$PATH
6- Preparar tu script de k6 en JS. En este caso, se llama k6-test.js
7- Ejecutar el script de k6 con el siguiente comando: ./k6 run --out web-dashboard=export=test-report.html k6-test.js (reemplazar k6-test.js con el nombre de tu script)
8- Dirigirse a la url generada por k6 para ver el dashboard en tiempo real, en este caso es: http://127.0.0.1:5665. (Cuando se termina la ejecución, no se puede acceder al panel)
9- Buscar en la carpeta donde se encuentra el script de k6 el archivo llamado test-report.html para visualizar un reporte como este:
10- Listo!
