### Supported tags and respective **``Dockerfile``** links
- `latest`, `5.7-hmap` [(Dockerfile)](https://github.com/zhw/docker-mysql-hmap/blob/master/5.7-hmap/Dockerfile)

### Base image: 
- `mysql:5.7`

### Features:
- Update mysql configurations for HAP:

  ```properties
  [client]
  default-character-set=utf8
  
  [mysql]
  default-character-set=utf8
  
  [mysqld]
  lower_case_table_names=1
  max_connections=500
  collation-server=utf8_unicode_ci
  init-connect='SET NAMES utf8'
  character_set_server=utf8
  sql_mode=STRICT_TRANS_TABLES,NO_ZERO_IN_DATE,NO_ZERO_DATE,ERROR_FOR_DIVISION_BY_ZERO,NO_AUTO_CREATE_USER,NO_ENGINE_SUBSTITUTION
  ```

  
