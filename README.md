# Extendi & Okteto @ KubeCon

kubectl -n dolly apply -f postgres-snapshot.yaml

kubectl -n dolly describe volumesnapshots

kubectl -n dolly delete -f postgres-snapshot.yaml

```SQL
CREATE TABLE users (
	id serial PRIMARY KEY,
	first_name VARCHAR ( 255 ) UNIQUE NOT NULL,
	last_name VARCHAR ( 255 ) NOT NULL,
	created_at TIMESTAMP NOT NULL DEFAULT NOW()
);
```

```SQL
INSERT INTO users (first_name, last_name) VALUES ('Ramiro', 'Berrelleza');
INSERT INTO users (first_name, last_name) VALUES ('Arsh', 'Sharma');
INSERT INTO users (first_name, last_name) VALUES ('Lapo', 'Elisacci');
```