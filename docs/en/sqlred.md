## How to handle with sql error problem.

Set up database and sql dialect in https://gejun123456.github.io/MyBatisCodeHelper-Pro/#/configure


### sql tag error, sql in mybatis sql is not complete, inspection and completion cant work，Plugin introduced @sql comment，set up sql prefix and suffix in the comment, so the sql is complete, inspection and completion will work fine.

![sqlTagNoError](https://gejun123456.coding.net/p/MyBatisCodeHelper-Pro/d/MyBatisCodeHelper-Pro/git/raw/master/screenshots/sqlTagNoError.gif)

If there is referenced select statement for sql tag, you can just alt enter the generate the @sql comment.
![addSqlComment](https://gejun123456.coding.net/p/MyBatisCodeHelper-Pro/d/MyBatisCodeHelper-Pro/git/raw/master/screenshots/addSqlComment.gif)

### when using if test, choose when May some of the condition is passed. only one pass in choose when. The plugin introduced @ignoreSql comment，if you need if test or choose when statment not pass, you can use it, so the sql will be correct.

请添加ignore注释 参考
![chooseWhenAutoComplete](https://gejun123456.coding.net/p/MyBatisCodeHelper-Pro/d/MyBatisCodeHelper-Pro/git/raw/master/screenshots/chooseWhenAutoComplete.gif)

### for ${} statement, the part can be any string, the sql can't be recognized. The plugin introduced $sql commment, you can add your real sql into the $sql comment to make sql correct. Sql statement after ${} can be recognized.

(2.7.6支持一键生成对应的sql)
![AddSqlAfter$](https://gejun123456.coding.net/p/MyBatisCodeHelper-Pro/d/MyBatisCodeHelper-Pro/git/raw/master/screenshots/AddSqlAfter$.gif)