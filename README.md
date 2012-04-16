# Reposit�rio para teste da PaaS Google AppEngine

### Para importar uma aplica��o para o Eclipse(3.7), tirando partido do Google Plugin
* File -> New -> Project -> Java Project
    * Indicar o nome do projeto que n�o necessita de ser igual ao da pasta onde os ficheiros da aplica��o se encontram;
    * Indicar a pasta onde se encontram os ficheiros com a aplica��o;
    * Finish;
* Project -> Properties -> Google -> App Engine
    * Marcar "Use Google App Engine";
* Project -> Properties -> Google -> Web Application
    * Marcar "This project has a WAR directory";
    * Indicar o caminho relativo para a pasta WAR;

### Para o caso de existirem erros de compila��o relacionados com:
* anota��es:
    1. Project -> Properties -> Java Compiler
        * Marcar "Enable project specific settings";
        * Indicar a vers�o adequada, superior ou igual � 1.5;

### Para o caso de existirem erros HTTP c�digo 500:
* java.lang.VerifyError:
    1.  Adicionar " -XX:-UseSplitVerifier" aos argumentos da m�quina virtual;
