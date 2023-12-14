# Graph Databases - graphle

Repository of group graphle for the "[Graph Databases](https://iiia.dei.unipd.it/education/database-2/)"
course, A.Y. 2023/2024. 

## Group members
| Surname   | Name      |
|-----------|-----------|
| Cardillo  | Vittorio	|
| Lenartavicius | Vaidas|
| Pallante  | Laura     |


## Dataset
**Start Point:** OpenFoodFacts [[Link](https://github.com/openfoodfacts)]  


**data:** Original dataset, not included in this repo, must be inserted in the data folder. [[Link](https://it.openfoodfacts.org/data)]

**data_2:** It is composed of 739411 elements with 35 attributes by a selection of the initial columns. To use it in the [[dataCleaning notebook](https://github.com/GreedyJacques/graphle/blob/main/code/dataCleaning.ipynb)], unzip this file into the data folder. [[Link](https://github.com/GreedyJacques/graphle/blob/main/data/data_2.zip)]

**Taxonomies:** OpenFoodFacts taxonomies. [[Link](https://github.com/openfoodfacts/openfoodfacts-server/tree/main/taxonomies)]

**data_2 attributes:**

* "product_name"
* "packaging_tags"
* "brands"
* "brands_tags"
* "labels_en"
* "countries_en"
* "ingredients_tags"
* "serving_size"
* "additives_n"
* "additives_tags"
* "nutriscore_score"
* "nutriscore_grade"
* "nova_group"
* "food_groups"
* "food_groups_tags"
* "brand_owner"
* "ecoscore_grade"
* "energy-kcal_100g"
* "energy_100g"
* "fat_100g"
* "saturated-fat_100g"
* "trans-fat_100g"
* "cholesterol_100g"
* "carbohydrates_100g"
* "sugars_100g"
* "fiber_100g"
* "proteins_100g"
* "salt_100g"
* "sodium_100g"
* "vitamin-a_100g"
* "vitamin-c_100g"
* "calcium_100g"
* "iron_100g"

## Repository guide

### Ontology

Model: [[graphleontology.ttl](https://github.com/GreedyJacques/graphle/blob/main/data/graphleontology.ttl)]

Draw.io: [[GraphleOntology.drawio](https://github.com/GreedyJacques/graphle/blob/main/docs/GraphleOntology.drawio)] - [[draw.io](draw.io)]

Png: [[GraphleOntology.png](https://github.com/GreedyJacques/graphle/blob/main/docs/GraphleOntology.png)]

### Jupyter Notebook (cleaning, ingestion, serialization)

Notebook: [[dataCleaning.ipynb](https://github.com/GreedyJacques/graphle/blob/main/code/dataCleaning.ipynb)]

### Serialization

RDF Serialization: [[food_database.ttl](https://github.com/GreedyJacques/graphle/blob/main/data/foodDB/food_database.ttl)]

RDF Serialization w/Ontology: [[food_database_with_onto.ttl](https://github.com/GreedyJacques/graphle/blob/main/data/foodDB/food_database_with_onto.ttl)]

### Query

Txt format: [[Queries.txt](https://github.com/GreedyJacques/graphle/blob/main/docs/Queries.txt)]

Excel format (more readable): [[Queries.xlsx](https://github.com/GreedyJacques/graphle/blob/main/docs/Queries.xlsx)]

Query results: [[QueriesResults](https://github.com/GreedyJacques/graphle/blob/main/docs/QueryResults/)]

## Notes

- The jupyter notebook is set to serialize 10.000 entries from the starting dataset (takes 20 minutes and generates a 20 Mb file);
- For the presentation of the project we would like to serialize a bigger portion of the dataset for more accurate data analytics;
- When opening the ontology in Protege the eulersharp countries ontology import sometimes fails, but succeeds after at most a couple of re-tries. 
