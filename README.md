# showing-the-BDD-Scenario-for-LISTING-ALL-PRODUCTS
Scenario: Listing all products
  Given the following products
    | name      | category | available |
    | ToyCar    | Toys     | true      |
    | BoardGame | Games    | true      |
  When I list all products
  Then I should see 2 products
