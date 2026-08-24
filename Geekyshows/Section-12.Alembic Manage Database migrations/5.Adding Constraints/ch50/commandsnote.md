- Initialize a new Alembic environment in the specified directory. This sets up the configuration files and script directory needed for migrations.

  ```bash 
  alembic init [directory]
  ```

- Create a new migration script.
  
  - Use -m to add a message describing the migration.
  
  - Add --autogenerate to automatically generate migration code based on model and database differences.

  ```bash
  alembic revision -m "message" [--autogenerate]
  ```

- Apply migrations up to the specified revision (e.g., head for the latest). This updates the database schema to the desired state.
 
  ```bash
  alembic upgrade [revision]
  ```

- This command upgrades your database schema forward by two migration steps from the current revision, applying the next two migrations in sequence

  ```bash
  alembic upgrade +2
  ```

- Revert migrations down to the specified revision, effectively rolling back schema changes.
  
  ```bash
  alembic downgrade [revision]
  ```

- This command downgrades (rolls back) your database schema by one migration step from the current revision, reverting the most recent migration

  ```bash
  alembic downgrade -1
  ```

- Display the current revision(s) applied to the database.

  ```bash
  alembic current
  ```

- Show the list of all migration scripts in chronological order.
  
  ```bash
  alembic history
  ```

- Check if there are pending upgrade operations when using autogenerate (available in newer versions).

  ```bash
  alembic check
  ```

- List available migration environment templates for initializing new projects.

  ```bash
  alembic list_templates
  ```
