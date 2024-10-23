[https://myacaddemy.oracle.com/](https://academy.oracle.com/)  
[https://iacademy2.oracle.com/](https://iacademy2.oracle.com/)

Databáze
* kolekce v tabulce

Identifikátory:
* P = Primary key
* F = Foreign (cizí) key
* PF = 
* U = unique, nelze mít 2 stejný hodnoty

Datové typy:
* NUMBER(x,y) = x: celkový počet míst (s desetinnými), y: počet desetinných míst
* VARCHAR(x) = string o délce x
* VARCHAR2(x) = 2.gen string
* DATE = uložení data

Pojmy
* Tabulka - zákl. úložná struktura (entita)
* sloupec - jeden druh dat v tabulce (atribut)
* řádek - data pro jednu instanci tabulky (instance)
* pole - jedna hodnota v průsečíku řádku a sloupce (hodnota), pokud není určena -> null
* primární klíč - unikátní identifikátor každého řádku
* cizí klíč - sloupec odkazující na primární klíč v jiné tabulce (relace)

Basic DB schéma
<br>
<img width="500px" src="https://github.com/FOFOLA1/DB2_Rehacek/blob/main/test.png">

Příkazy
* DML - manipulace s daty, insert, update, delete, merge
* DDL - create. alter, drop, rename
* TCL - commit, rollback, savepoint
* DCL - grant, rewoke

Transakce v RDBMS
* ACID
* Atomicita
* konzistence
* izolace
* Trvalost

DB v konzistentním stavu
<br>
```
set transaction ...
  UPDATE ...
  INSERT
  INSERT
commit; //potvrdí transakci
rollback; //vrátí zpět před transakci
```
<br>
Ukázka syntaxe

```
SELECT LAST_NAME FROM EMPLOYES
SELECT LAST_NAME, SALARY, SALARY + 300 //neměníme data tabulky, pouze výstup
FROM EMPLOYEE
```

Aliasy
<br>
```
SELECT LAST_NAME AS NAME
```
