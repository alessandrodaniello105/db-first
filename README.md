DB-first
===

id            |         INT           |   PRIMARY_KEY - NOT NULL/UNIQUE - AUTO-INCREMENT
<!-- name  |   VARCHAR(40)   |    -->
brand         |      VARCHAR(20)      |   NOT NULL 
model         |      VARCHAR(20)      |   NOT NULL
power         |   SMALLINT UNSIGNED   |   NOT NULL
transmission  |        CHAR(1)        |   NOT NULL
fuel          |      VARCHAR(10)      |   NOT NULL /* fi.'diesel', 'other fuel' */
engineCapacity|       VARCHAR(4)      |   NOT NULL /* fi.'1600' */
driveType     |        CHAR(1)        |   NOT NULL, DEFAULT "2" /* 2 = 4x2 ; 4 = 4x4 */
type          |      VARCHAR(20)      |   NULL
features      |         TEXT          |   NULL
images        |      VARCHAR(35)      |   NOT NULL
location      |      VARCHAR(40)      |   NOT NULL
price         |   MEDIUMINT UNSIGNED  |   NOT NULL
yearReg       |         YEAR          |   NOT NULL
dateAdded     |         DATE          |   NOT NULL
condition     |      VARCHAR(15)      |   NULL
euroNorm      |        CHAR(1)        |   NULL
colorExt      |      VARCHAR(20)      |   NULL
colorIxt      |      VARCHAR(20)      |   NULL
doors         |       VARCHAR(3)      |   NULL
consumption   |       VARCHAR()       |   NULL
mileage       |   MEDIUMINT UNSIGNED  |   NOT NULL
deductible    |        CHAR(1)        |   NOT NULL - DEFAULT('0')