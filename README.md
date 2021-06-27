# DDD event-driven

Boiler plate for Domain driven and event driven service
Inspired by the work from Architecture Patterns with Python (https://www.oreilly.com/library/view/architecture-patterns-with/9781492052197/)

- Domain centric with uow and repository pattern
- Event driven (internal event loop and external message bus)
- Dependency injection for external connector (among those : orm, object storage, authorization server)
- Production grade API (pagination, JWT authentication, RESTful)

## Developpement

```bash
git clone git@github.com:augustinbarbe/allocation_domain.git
cd allocation_domain/
```

Run the application stack for local development ( support hot reload):
Requires docker

```bash
make run
```

Delete the stack (including database)

```bash
make clean
```

Run unit tests

```
make test
```


## Entrypoints :
The service can be consumed from a REST Api