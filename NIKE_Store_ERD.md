# NIKE Store

```mermaid
erDiagram 
Products{
int ProductID PK
string ProductName
int Price
string Size
}
Customers{
int CustomerID PK
string Name

}
Orders{
int OrderID PK
int CustomerID FK

}

Inventory{
string ProductID FK
int InStock

}
Customers ||..o{Orders :have
Orders }o..|| Products : have
Products ||..||Inventory: in
