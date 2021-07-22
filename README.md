
Write a Product GraphQL API to provide the product data.


### Product Table
product_id | product_name | product_description | list_price | sale_price    
--- | --- | --- | --- |---      
p123 | {"en_CA": "PAW Patrol Boys' Toddler Rubber Rain Boots", "fr_CA": "Botte de pluie La Pat' Patrouille en caoutchouc pour bambins"} | {"en_CA": ""• This Paw Patrol rain boot for toddlers is ideal for spring time.<br>• It is completely waterproof, entirely made of rubber, comfortable and has easy pull-on handles.<br>• Perfect for jumping in puddles and playing  outside on rainy days!"", "fr_CA": ""• Cette botte de pluie La Pat' Patrouille pour bambins est idéale pour le printemps<br>• Construction complètement en caoutchouc. La botte est imperméable et possède des poignées pour mettre la botte plus facilement<br>• Parfaite pour sauter dans les flaques d'eau et jouer dehors les jours de pluie!"} | 29.99 | 19.99     

### GraphQL query to support.

```
{
  products(ids:["p123"]){
    id
    name{
      en_CA
      fr_CA
    }
    description{
      en_CA
      fr_CA
    }
    list_price
    sale_price
  }
}
```