lecture-14

Home task lecture 14:
0. On git repo.
1. Base on hometask 13.
2. README with the task.
3. Add JDBC template from spring.
4. Add 1 DAO implementation with JDBC template.
5. Add 1 DAO implementation with Named JDBC template.

NOTE: should be used: queryForObject

Additional for 10
6. Docker-compose.
7. Tests for DAO.

What's done:
- added README.md;
- added JdbcTemlate to ProducersDAO, CategoriesDAO
- added NamedParameterJdbcTemplate to GoodsDAO.
All dao using BeanPropertyRowMapper. DAO using queryFor 
object() and query() on SELECT. DAO using update() on insert, update, delete.

-Added docker compose file at src/main/resources/docker/docker-compose.yml
-Added tests for CategoriesDAO

Run Docker then run Liquibase:
$cd /PATH/src/main/resources/docker/
$docker-compose up
$cd ../../../..
$mvn liquibase:update

Then start the App