# Comandos para configurar o compilador do TypeScript

+ Na pasta do projeto, crie o arquivo **tsconfig.json**.
+ Digite o seguinte:
    ```JSON
    {
        "compilerOptions": {
            "outFile": "main.js"
        }
    }
    ```

+ Depois, va no arquivo package.json e mude o scipt que faz o build do projeto. Mude para **tsc**.

+ Ao temtar colocar uma das funções criadas para ser assincrona, o VS Code acusarar um erro pois o ES3 não tem suporte para essa função. Dessa forma,  é nescessario configurar o compilador para nos retorna um código em uma versão mais atual do javascript. 

+ Para resolver esse problema, basta ir no arquivo **tsconfig.json** e adicionar o seguinte código:
    ```json
    {
        "compilerOptions": {
            "outFile": "main.js",
            "target": "EsNext"
        }
    }
    ```

+ Feito isso, o compilador compilarar o código TypeScript para a versão mais atual do Javascript.