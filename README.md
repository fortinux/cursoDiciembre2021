# Curso de Python diciembre del 2021

## Inicializar repositorio utilizando git
- Comandos en la terminal    

- Configuramos nuestro nombre de usuario:
`git config --global user.name "usuario"`    
    
- Configuramos nuestra dirección de e-mail:    
`git config --global user.email "usuario@email.com"`
    
- Creamos una llave SSH:    
`ssh-keygen -t rsa -C "usuario@email.com"`
    
- Copiamos la clave SSH en nuestra cuenta en GIT https://github.com/settings/ssh:
`cat ~/.ssh/id_rsa.pub`    
    
- Controlamos si esta correcta:
`ssh -T git@github.com`  
    
- iniciar git
`git init`   
     
- agregar el repositorio creado anteriormente en el cvs    
`git remote add origin git@github.com:fortinux/curso2021Nov15.git`    
`git fetch origin main`    
    
- obtener los ficheros del repositorio apenas creados    
`git pull origin main`     
`git status`        
    
- crear fichero .gitignore con los ficheros que no se quieren subir al repositorio    
`vim .gitignore`     
    
- agregar los ficheros al commit    
`git add .`    
`git commit -m "clase 1"`    
    
- hacer el commit para subir los ficheros al repositorio    
`git push origin master`

- Error dirección del repositorio
git remote set-url origin git@github.com:fortinux/curso2021Nov15.git
git push -u origin HEAD:main