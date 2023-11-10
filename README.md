DB-first
===

id            |          INT          |   PRIMARY_KEY - NOT NULL/UNIQUE - AUTO-INCREMENT
<!-- name  |   VARCHAR(40)   |    -->
brand         |      VARCHAR(20)      |   NOT NULL /* 'mercedes-benz', 'fiat' */
model         |      VARCHAR(20)      |   NOT NULL /* '5008', 'Multipla' */
power         |   SMALLINT UNSIGNED   |   NOT NULL /* 34, 129 hp  */
owners        |   TINYINT UNSIGNED    |   NOT NULL /* (past owner(s)) 2, 10 */
id_owner      |          INT          |   NOT NULL
transmission  |        CHAR(1)        |   NOT NULL /* M = manual, A = automatic, S = semi-automatic */
supply        |      VARCHAR(10)      |   NOT NULL /* 'diesel', 'other fuel' */
engineCapacity|       VARCHAR(4)      |   NOT NULL /* '1600' (-> 1.6) kW */
driveType     |        CHAR(1)        |   NOT NULL, DEFAULT "2" /* 2 = 4x2 ; 4 = 4x4 */
type          |      VARCHAR(20)      |   NULL /* 'Coupe', 'Cabriolet', 'Other type' */
features      |         TEXT          |   NULL /* 'Wi-fi, cigarette lighter, ...' */
images        |      VARCHAR(35)      |   NOT NULL /* peugeout-208-red-front.jpg */
location      |      VARCHAR(40)      |   NOT NULL /* 'Cinisello Balsamo, Milan 20092' */
<!-- price         |   MEDIUMINT UNSIGNED  |   NOT NULL /* 15000, 1000, 999999 */ -->
price         |   MEDIUMINT UNSIGNED  |   NOT NULL /* 15000, 1000, 999999 */
yearReg       |         YEAR          |   NOT NULL /* 2015 */
dateAdded     |         DATE          |   NOT NULL /* 2023-11-09 */
condition     |      VARCHAR(15)      |   NULL /* 'used', 'near mint' */
euroNorm      |        CHAR(1)        |   NULL /* '4', '6' (-> Euro 4/Euro 6) */
colorExt      |      VARCHAR(21)      |   NULL /* 'Light cornflower blue' */
colorIxt      |      VARCHAR(21)      |   NULL /* 'Tan' */
doors         |       VARCHAR(3)      |   NULL /* '4/5' */
consumption   |       VARCHAR()       |   NULL /* '5.5 l/100km', '6.5 l/100km (city) - 4.5 l/100km' */
mileage       |   MEDIUMINT UNSIGNED  |   NOT NULL /* '1000', '420', '65536' (-> 1000 km/621 mi) */
deductible    |        CHAR(1)        |   NOT NULL - DEFAULT('0')
vin           |      VARCHAR(17)      |   NOT NULL
license plate |      VARCHAR(10)      |   NOT NULL
nationalities |      VARCHAR(20)      |   NOT NULL /* (brand nationality) */