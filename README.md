# protocole-http
## Schneider Arthur
## Il n'y a pas d'instalation essentiels

## 2. Notion d'adresse Web 
### 1 Trouvez la syntaxe des URI permettant :

#### 1.1 D'envoyer un mail (mais ne l'envoyez pas !) avec sujet du mail fourni (Ex : mail à jerome.cutrona@univ-reims.fr avec le sujet J'aime le Web)  
    mailto:jerome.cutrona@univ-reims.fr?subject=j'aime le Web

#### 1.2 d'accéder à un répertoire partagé par un serveur ftp en anonyme (Ex : ftp.sunet.se ou ftp.proxad.net)
    ftp://ftp.sunet.se

#### 1.3 d'accéder à un répertoire local sur votre poste de travail (Ex : /tmp sur Linux) 
file:///tmp

### 2 Donnez les valeurs des éléments constitutifs des URI qui suivent :

#### 2.1 https://example.com/
    https = scheme
    example.com = host
    / = path

#### 2.2 https://www.iut-rcc.fr/media-files/30677/but-info.pdf
    https = scheme
    www.iut-rcc.fr = host
    media-files/30677/but-info.pdf = path

#### 2.3 https://iut-info.univ-reims.fr/users/cutrona/intranet/installation-configuration/ubuntu-opennebula/index.html#objectifs-de-la-seance
    https = scheme
    iut-info.univ-reims.fr = host
    /users/cutrona/intranet/installation-configuration/ubuntu-opennebula/index.html = path
    objectifs-de-la-seance = fragment

#### 2.4 http://demo.ad-urca.univ-reims.fr/?info
    http = scheme
    demo.ad-urca.univ-reims.fr = host
    / = path
    ?info = query

#### 2.5 mysql://app:!ChangeMe!@127.0.0.1:3306/app?serverVersion=8&charset=utf8mb4
    mysql = scheme
    app:!ChangeMe!@127.0.0.1:3306 = userinfo
    /app = path
    ?serverVersion=8&charset=utf8mb4 = query

#### 2.6 https://www.univ-reims.fr/formation/catalogue-de-formation/but-informatique,23515,38949.html?args=R9qFsCnMmKDtxCa17YTDkHVqaqbfYRXwwTnCVt2witCDUIiVoUdkeMDp%2AXGEGm2SMIhvMbuZ3_kOrRxvJlk6dOorIryuNioRCyFFyPAvhl9tCdwYdtHRrwAvNC1tDg_H&formation_id=17#formationDetailDecriptions 
    https = scheme
    www.univ-reims.fr  = host
    /formation/catalogue-de-formation/ but-informatique,23515,38949.html = path
    ?args=R9qFsCnMmKDtxCa17YTDkHVqaqbfYRXwwTnCVt2witCDUIiVoUdkeMDp%2AXGEGm2SMIhvMbuZ3_kOrRxvJlk6dOorIryuNioRCyFFyPAvhl9tCdwYdtHRrwAvNC1tDg_H&formation_id=17 = query
    #formationDetailDecriptions = fragment

## 3.3.1 Ressource principale 
### 5.1 Donnez le nom de la ressource principale 
    La resource principale est /

### 5.2 Donnez la nature de la ressource principale 
    la ressource principale est une page HTML

### 5.3 Expliquez la présence de la ressource favicon.ico*
    une page HTML recherche toujours le favicon.ico même ci il n'existe pas

