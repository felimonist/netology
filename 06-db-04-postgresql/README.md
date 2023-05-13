Задание 1.


![slave](https://github.com/felimonist/netology/06-db-04-postgresql/blob/main/img/1.JPG)

вывода списка БД
подключения к БД
![slave](https://github.com/felimonist/netology/06-db-04-postgresql/blob/main/img/1.2.JPG)

вывод списка таблиц
postgres=# \dtS
                    List of relations
   Schema   |          Name           | Type  |  Owner   
------------+-------------------------+-------+----------
 pg_catalog | pg_aggregate            | table | postgres
 pg_catalog | pg_am                   | table | postgres
 pg_catalog | pg_amop                 | table | postgres
 pg_catalog | pg_amproc               | table | postgres
 pg_catalog | pg_attrdef              | table | postgres
 pg_catalog | pg_attribute            | table | postgres
 pg_catalog | pg_auth_members         | table | postgres
 pg_catalog | pg_authid               | table | postgres
 pg_catalog | pg_cast                 | table | postgres
 pg_catalog | pg_class                | table | postgres
 pg_catalog | pg_collation            | table | postgres
 pg_catalog | pg_constraint           | table | postgres
 pg_catalog | pg_conversion           | table | postgres
 pg_catalog | pg_database             | table | postgres
 pg_catalog | pg_db_role_setting      | table | postgres
 pg_catalog | pg_default_acl          | table | postgres
 pg_catalog | pg_depend               | table | postgres
 pg_catalog | pg_description          | table | postgres
 pg_catalog | pg_enum                 | table | postgres
 pg_catalog | pg_event_trigger        | table | postgres
 pg_catalog | pg_extension            | table | postgres
 pg_catalog | pg_foreign_data_wrapper | table | postgres
 pg_catalog | pg_foreign_server       | table | postgres
 pg_catalog | pg_foreign_table        | table | postgres
 pg_catalog | pg_index                | table | postgres
 pg_catalog | pg_inherits             | table | postgres
 pg_catalog | pg_init_privs           | table | postgres
 pg_catalog | pg_language             | table | postgres
 pg_catalog | pg_largeobject          | table | postgres
 pg_catalog | pg_largeobject_metadata | table | postgres
 pg_catalog | pg_namespace            | table | postgres
 pg_catalog | pg_opclass              | table | postgres
 pg_catalog | pg_operator             | table | postgres
 pg_catalog | pg_opfamily             | table | postgres
 pg_catalog | pg_partitioned_table    | table | postgres
 pg_catalog | pg_policy               | table | postgres
 pg_catalog | pg_proc                 | table | postgres
 pg_catalog | pg_publication          | table | postgres
 pg_catalog | pg_publication_rel      | table | postgres
 pg_catalog | pg_range                | table | postgres
 pg_catalog | pg_replication_origin   | table | postgres
 pg_catalog | pg_rewrite              | table | postgres
 pg_catalog | pg_seclabel             | table | postgres
 pg_catalog | pg_sequence             | table | postgres
 pg_catalog | pg_shdepend             | table | postgres
 pg_catalog | pg_shdescription        | table | postgres
 pg_catalog | pg_shseclabel           | table | postgres
 pg_catalog | pg_statistic            | table | postgres
 pg_catalog | pg_statistic_ext        | table | postgres
 pg_catalog | pg_statistic_ext_data   | table | postgres
 pg_catalog | pg_subscription         | table | postgres
 pg_catalog | pg_subscription_rel     | table | postgres
 pg_catalog | pg_tablespace           | table | postgres
 pg_catalog | pg_transform            | table | postgres
 pg_catalog | pg_trigger              | table | postgres
 pg_catalog | pg_ts_config            | table | postgres
 pg_catalog | pg_ts_config_map        | table | postgres
 pg_catalog | pg_ts_dict              | table | postgres
 pg_catalog | pg_ts_parser            | table | postgres
 pg_catalog | pg_ts_template          | table | postgres
 pg_catalog | pg_type                 | table | postgres
 pg_catalog | pg_user_mapping         | table | postgres
(62 rows)
вывод описания содержимого таблиц
postgres=# \dS+
                                            List of relations
   Schema   |              Name               | Type  |  Owner   | Persistence |    Size    | Description 
------------+---------------------------------+-------+----------+-------------+------------+-------------
 pg_catalog | pg_aggregate                    | table | postgres | permanent   | 56 kB      | 
 pg_catalog | pg_am                           | table | postgres | permanent   | 40 kB      | 
 pg_catalog | pg_amop                         | table | postgres | permanent   | 80 kB      | 
 pg_catalog | pg_amproc                       | table | postgres | permanent   | 64 kB      | 
 pg_catalog | pg_attrdef                      | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_attribute                    | table | postgres | permanent   | 456 kB     | 
 pg_catalog | pg_auth_members                 | table | postgres | permanent   | 40 kB      | 
 pg_catalog | pg_authid                       | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_available_extension_versions | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_available_extensions         | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_cast                         | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_class                        | table | postgres | permanent   | 136 kB     | 
 pg_catalog | pg_collation                    | table | postgres | permanent   | 240 kB     | 
 pg_catalog | pg_config                       | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_constraint                   | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_conversion                   | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_cursors                      | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_database                     | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_db_role_setting              | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_default_acl                  | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_depend                       | table | postgres | permanent   | 488 kB     | 
 pg_catalog | pg_description                  | table | postgres | permanent   | 376 kB     | 
 pg_catalog | pg_enum                         | table | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_event_trigger                | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_extension                    | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_file_settings                | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_foreign_data_wrapper         | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_foreign_server               | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_foreign_table                | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_group                        | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_hba_file_rules               | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_index                        | table | postgres | permanent   | 64 kB      | 
 pg_catalog | pg_indexes                      | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_inherits                     | table | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_init_privs                   | table | postgres | permanent   | 56 kB      | 
 pg_catalog | pg_language                     | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_largeobject                  | table | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_largeobject_metadata         | table | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_locks                        | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_matviews                     | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_namespace                    | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_opclass                      | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_operator                     | table | postgres | permanent   | 144 kB     | 
 pg_catalog | pg_opfamily                     | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_partitioned_table            | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_policies                     | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_policy                       | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_prepared_statements          | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_prepared_xacts               | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_proc                         | table | postgres | permanent   | 688 kB     | 
 pg_catalog | pg_publication                  | table | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_publication_rel              | table | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_publication_tables           | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_range                        | table | postgres | permanent   | 40 kB      | 
 pg_catalog | pg_replication_origin           | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_replication_origin_status    | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_replication_slots            | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_rewrite                      | table | postgres | permanent   | 656 kB     | 
 pg_catalog | pg_roles                        | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_rules                        | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_seclabel                     | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_seclabels                    | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_sequence                     | table | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_sequences                    | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_settings                     | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_shadow                       | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_shdepend                     | table | postgres | permanent   | 40 kB      | 
 pg_catalog | pg_shdescription                | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_shmem_allocations            | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_shseclabel                   | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_stat_activity                | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_all_indexes             | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_all_tables              | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_archiver                | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_bgwriter                | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_database                | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_database_conflicts      | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_gssapi                  | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_progress_analyze        | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_progress_basebackup     | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_progress_cluster        | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_progress_create_index   | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_progress_vacuum         | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_replication             | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_slru                    | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_ssl                     | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_subscription            | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_sys_indexes             | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_sys_tables              | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_user_functions          | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_user_indexes            | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_user_tables             | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_wal_receiver            | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_xact_all_tables         | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_xact_sys_tables         | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_xact_user_functions     | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stat_xact_user_tables        | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_statio_all_indexes           | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_statio_all_sequences         | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_statio_all_tables            | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_statio_sys_indexes           | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_statio_sys_sequences         | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_statio_sys_tables            | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_statio_user_indexes          | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_statio_user_sequences        | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_statio_user_tables           | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_statistic                    | table | postgres | permanent   | 248 kB     | 
 pg_catalog | pg_statistic_ext                | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_statistic_ext_data           | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_stats                        | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_stats_ext                    | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_subscription                 | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_subscription_rel             | table | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_tables                       | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_tablespace                   | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_timezone_abbrevs             | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_timezone_names               | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_transform                    | table | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_trigger                      | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_ts_config                    | table | postgres | permanent   | 40 kB      | 
 pg_catalog | pg_ts_config_map                | table | postgres | permanent   | 56 kB      | 
 pg_catalog | pg_ts_dict                      | table | postgres | permanent   | 48 kB      | 
 pg_catalog | pg_ts_parser                    | table | postgres | permanent   | 40 kB      | 
 pg_catalog | pg_ts_template                  | table | postgres | permanent   | 40 kB      | 
 pg_catalog | pg_type                         | table | postgres | permanent   | 120 kB     | 
 pg_catalog | pg_user                         | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_user_mapping                 | table | postgres | permanent   | 8192 bytes | 
 pg_catalog | pg_user_mappings                | view  | postgres | permanent   | 0 bytes    | 
 pg_catalog | pg_views                        | view  | postgres | permanent   | 0 bytes    | 
(129 rows)

выход
\q


Задание 2.

![slave](https://github.com/felimonist/netology/06-db-04-postgresql/blob/main/img/2.JPG)

![slave](https://github.com/felimonist/netology/06-db-04-postgresql/blob/main/img/2.1.JPG)

Задание 3.

![slave](https://github.com/felimonist/netology/06-db-04-postgresql/blob/main/img/3.JPG)
Можно изначально исключить "ручное" разбиение при проектировании таблицы orders, если использовать декларативное секционирование с предложением PARTITION BY.

Задание 4.

![slave](https://github.com/felimonist/netology/06-db-04-postgresql/blob/main/img/4.JPG)

Для уникальности значения столбца title добавим строку в бэкап

ALTER TABLE ONLY public.orders ADD CONSTRAINT title_unique UNIQUE (title);

