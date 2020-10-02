# Golang To-do App

This project is simple CRUD To-Do List application built in golang and using Postgresql.

## Pre-requisite
1. Install golang v1.11 or above.
2. Install PostgreSQL v10 or above.

## PostgreSQL Table
```sql
CREATE EXTENSION IF NOT EXISTS "uuid-ossp";
```

```sql
CREATE TABLE IF NOT EXISTS todos (
  id UUID NOT NULL DEFAULT uuid_generate_v4(),
  text TEXT,
  checked BOOLEAN
);
```

## Next steps
- clone this repository
- run program `go run main.go`
- open browser `http://localhost:8000`