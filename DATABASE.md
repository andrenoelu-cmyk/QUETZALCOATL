[[IDENTITY]]
# QUETZALCOATL — Database Specification

## 1. Purpose

QUETZALCOATL uses a local SQLite database to persist the information required by
the application.

The database must remain simple, local, portable, and dependency-light.

The database is not intended to become a general-purpose knowledge base.

For version 0.1, QUETZALCOATL only needs to persist user tasks/events and the
minimum metadata required to manage them safely.

---

## 2. Database technology

Database:

- SQLite
- Local file
- No external database server
- No cloud synchronization
- No network database
- No unnecessary ORM requirement

The database file should be stored inside QUETZALCOATL's application data
directory and must not be placed inside the user's file organization
directories.

The exact path is an implementation decision.

---

## 3. Core concept

QUETZALCOATL does not strictly distinguish between:

- tasks
- reminders
- events
- appointments
- important dates

For version 0.1, all of these are represented as a single type of entry.

The important information is:

- what it is
- when it happens
- whether it has been completed
- when it was created
- optionally, additional notes

The application should avoid unnecessary categorization.

---

# 4. Schema

## `entries`

Main table containing everything the user wants QUETZALCOATL to remember.

| Column       | Type    | Required | Description                                     |
| ------------ | ------- | -------: | ----------------------------------------------- |
| `id`         | INTEGER |      YES | Unique identifier                               |
| `title`      | TEXT    |      YES | Short description of the entry                  |
| `date`       | TEXT    |       NO | Date associated with the entry, ISO 8601 format |
| `time`       | TEXT    |       NO | Optional time, `HH:MM`                          |
| `completed`  | INTEGER |      YES | `0` for incomplete, `1` for completed           |
| `notes`      | TEXT    |       NO | Optional additional information                 |
| `created_at` | TEXT    |      YES | Creation timestamp                              |
| `updated_at` | TEXT    |      YES | Last modification timestamp                     |

### Recommended SQL

```sql
CREATE TABLE entries (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    title TEXT NOT NULL,
    date TEXT,
    time TEXT,
    completed INTEGER NOT NULL DEFAULT 0,
    notes TEXT,
    created_at TEXT NOT NULL,
    updated_at TEXT NOT NULL
);