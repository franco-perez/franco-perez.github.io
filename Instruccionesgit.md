

# Como aprender Markdown?

[nombredellink](https://link)

Haz click en [Markdown](https://docs.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax) para acceder a un breve tutorial de markdown

# La forma de hacer graficos livianos y programados

para mayor informacion revisa el archivo de extension .md

<img src='https://g.gravizo.com/svg?
 digraph G {
    rankdir=LR;
    Computer->Github [ label="push" ];
    Github->Computer [ label="pull" ];    
    } 
'/>

# flujo de trabajo en Github

a continuacion se muestra una foto del flujo de trabajo en git

![Workflow-git](  /images/Workflow_git.png) 
slash permite que github adhiera la linea al directorio


Workspace   |  staggingArea | localRepository|remoterepository \
git add       | git commit     | git pushsh 

``` bash
user@host:~$  git status  #este comando sirve para ver el estado de github
user@host:~$ git add . #comando para agregar archivos modificados al stage area 
user@host:~$ git coomit . #comando para agregar archivos modificados al stage area
```


<img src='https://g.gravizo.com/svg?
 digraph G {
   main -> parse -> execute;
   main -> init;
   main -> cleanup;
   execute -> make_string;
   execute -> printf
   init -> make_string;
   main -> printf;
   execute -> compare;
 }
'/>


# Graphviz 
- dia
- gravizo
- mermaid
- graphviz (dot)