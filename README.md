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

## 3.3.2 Ressources liées 
### 4.1 « style.css »
    elle est utiliser est demander par http://cutrona/but/s2/protocole-http/

### 4.2 « correction.js »
    elle est utiliser est demander par http://cutrona/but/s2/protocole-http/

### 4.3  « URI_syntax_diagram.svg »
    elle est utiliser est demander par http://cutrona/but/s2/protocole-http/

### 4.4 « timer.png » 
    elle est utiliser est demander par http://cutrona/css/style.css

## 4.2 Visualisation des requêtes HTTP 
### 2 Observez la requête et expliquez tous ses éléments constitutifs
    GET /request/dump/ HTTP/1.1 = ligne de requête

    Host: demo.ad-urca.univ-reims.fr = adresse de la ressource
    User-Agent: Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:102.0) Gecko/20100101 Firefox/102.0 = info sur l'utilisateur (distribution, moteur de recherche)
    Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8 = reponse accepter
    Accept-Language: fr,fr-FR;q=0.8,en-US;q=0.5,en;q=0.3 = langage accepter
    Accept-Encoding: gzip, deflate = encodage accepter
    Referer: http://cutrona/ = referance de la page
    Connection: keep-alive = grader la connection etablie
    Cookie: _ga=GA1.1.1454122362.1666786956; _ga_FXME7WP04L=GS1.1.1673023630.1.1.1673025872.0.0.0 = info dur l'utilisateur
    Upgrade-Insecure-Requests: 1 = 
    Pragma: no-cache = demande du serveur au niveau client
    Cache-Control: no-cache = controle du cache

### 4 Observez et expliquez les changements dans la requête transmise au serveur
    il n'y a pas de changemenet au niveaux de la requette

### 6 Observez et expliquez les changements dans la requête transmise au serveur
    les lignes Pragma et cookie on disparut

### 10 Observez et expliquez les changements dans la requête transmise au serveur
    la ligne des cookie n'est pas présenet car on a desactiver le cache