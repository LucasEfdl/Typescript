# Instalando o TypeScript
+ Primeiro inicilaize o npm: **npm init**

+ Depois você pod instalar ele globalmente ou localmente
    + globalmente: **npm install -g typescript**
    + localmente: **npm install --save-dev typescript**

+ Para compilar o codigo para JavaScript, use o seguinte comando: **npx tsc nome_do_arquivo.ts**

+ Ou, va no arquivo package.json e, em scripts, escreva o seguinte
    ```JSON
        {
            ...
            "scripts": {
                "build": "tsc index.ts"
            }
            ...
        }
    ```

+ Em seguida, va no terminal e digite **npm run build** e o codigo typescript será compilado para javascript.