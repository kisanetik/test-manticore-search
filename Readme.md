For bug testing with highlight on manticoresearch.

First run:
  docker-compose up -d
  docker-compose exec maria bash -c 'mysql -u root -pmysql < /data/dump.sql'
  docker-compose run manticore bash -c 'indexer --all'