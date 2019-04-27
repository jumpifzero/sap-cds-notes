# sap-cds-notes
Notes on using the sap/cds javascript package from SAP and the cds command

# Useful commands

## Initializing a new cds project

This will create a project with a service and database layers.

Create the folder where you want to initialize, `cd` into it then do:

```sh
cds init --modules db,srv
```

## Building your data models

```sh
cds build/all --clean
```

## Deploy schema to DB

_warning:_ The below command drops all the data in the database.

```sh
cds deploy --to sqlite:db/my-db-name.db
```

# Starting the REPL

The repl gives you a javascript console where you can interact with cds.

```sh
cds repl
```

## Starting the local OData server

```sh
cds serve all
```