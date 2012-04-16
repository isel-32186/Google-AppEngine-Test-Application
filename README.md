# Repositório para teste da PaaS Google AppEngine

### Para importar uma aplicação para o Eclipse(3.7), tirando partido do Google Plugin
* File -> New -> Project -> Java Project
    * Indicar o nome do projeto que não necessita de ser igual ao da pasta onde os ficheiros da aplicação se encontram;
    * Indicar a pasta onde se encontram os ficheiros com a aplicação;
    * Finish;
* Project -> Properties -> Google -> App Engine
    * Marcar "Use Google App Engine";
* Project -> Properties -> Google -> Web Application
    * Marcar "This project has a WAR directory";
    * Indicar o caminho relativo para a pasta WAR;

### Para o caso de existirem erros de compilação relacionados com:
* anotações:
    1. Project -> Properties -> Java Compiler
        * Marcar "Enable project specific settings";
        * Indicar a versão adequada, superior ou igual à 1.5;

### Para o caso de existirem erros HTTP código 500:
* java.lang.VerifyError:
    1.  Adicionar " -XX:-UseSplitVerifier" aos argumentos da máquina virtual;
