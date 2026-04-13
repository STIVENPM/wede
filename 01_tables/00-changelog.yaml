databaseChangeLog:
  - changeSet:
      id: 01_tables
      author: mertinez.stiven@gmail.com
      context: billing
      labels: HU_02
      comment: person creation
      changes:
        - tagDatabase:
            tag: v1.0.1
        - sqlFile:
            path: 01_tables/01-create-person.sql
            stripComments: false
            splitStatements: false
      rollback:
        - sqlFile:
            path: 11_rollbacks/01_tables/01-create-person-rollback.sql
            stripComments: false
            splitStatements: false

  - changeSet:
      id: 02_inserts_person
      author: mrtinez.stiven@gmail.com
      context: billing
      labels: HU_02
      comment: insert initial data into person
      changes:
        - sqlFile:
            path: 02_inserts/02-inserts-person.sql
            stripComments: false
            splitStatements: true
      rollback:
        - sqlFile:
            path: 11_rollbacks/02_inserts/02-inserts-person-rollback.sql
            stripComments: false
            splitStatements: true