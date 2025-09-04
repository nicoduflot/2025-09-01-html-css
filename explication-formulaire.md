# Traitement des formulaires
---

## Traitement des données via PHP

Les données sont stockées dans des variables globales : 

```$_GET``` pour les données envoyées avec ```method="get"```
```$_POST``` pour les données envoyées avec ```method="post"```

```php
/* en php le traitement des variables globales */
$_GET['search' => 'toto', 'formSub' => true];

$_POST['search' => 'toto', 'formSub' => true];

if(isset($_GET['formSub']) && $_GET['formSub']){
    /* code traitement et vérification du formulaire */
}

if(isset($_POST['formSub']) && $_GET['formSub']){
    /* code traitement et vérification du formulaire */
}
```