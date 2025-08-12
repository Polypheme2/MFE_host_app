1 - INTRODUCTION :
    - This project (named host_app) is the main project of the micro-frontend application we intent develop
    - So, this project will be responsible of displaying microfrontend
    - This project (named host_app) is using native federation as micro-frontend developpement tool (instead of module federation)

2 -DEVELOPPEMENT ENVIRONNEMENT CARACTERISTICS :
    ng v

            _                      _                 ____ _     ___
            / \   _ __   __ _ _   _| | __ _ _ __     / ___| |   |_ _|
        / △ \ | '_ \ / _` | | | | |/ _` | '__|   | |   | |    | |
        / ___ \| | | | (_| | |_| | | (_| | |      | |___| |___ | |
        /_/   \_\_| |_|\__, |\__,_|_|\__,_|_|       \____|_____|___|
                        |___/
            

        Angular CLI: 17.0.0
        Node: 18.20.8
        Package Manager: npm 10.8.2
        OS: linux x64

        Angular: 
        ... 

        Package                      Version
        ------------------------------------------------------
        @angular-devkit/architect    0.1700.0 (cli-only)
        @angular-devkit/core         17.0.0 (cli-only)
        @angular-devkit/schematics   17.0.0 (cli-only)
        @schematics/angular          17.0.0 (cli-only)

3 - NOTE :
    - If you have a look at git, you will sie that commits name are following step by step how the project has been built.

3 - DEVELOPPEMENT PROCESS : 
    - step1 : Create a folder named native_federation
        steph@steph-To-be-filled-by-O-E-M:~/homework_Angular/native_federation
    - step2 - Creation of app host into /homework_Angular/native_federation
        command line:
            ng new host_app
    - step3 - Library installation of native federation into host_app
        cd host_app
        npm i @angular-architects/native-federation@17.0.0
    - step4 - Make this project (host_app) capable of handling federation dynamic-host (--type dynamic-host is meaning that this project aime is to diplay micro front ends)
        ng generate @angular-architects/native-federation:init --project host_app --port 4200 --type dynamic-host