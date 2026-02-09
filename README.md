# Corrode

A Django-like web framework for Rust with ORM, admin interface,
authentication, forms, routing, and migrations.

Built on top of [oxide-sql](https://github.com/LeakIX/oxide-sql) for
type-safe SQL.

## Features

- **Django-like ORM**: Familiar QuerySet API, Model trait, and Managers
- **Admin Interface**: Automatic CRUD admin with Bootstrap 5 UI
- **Database Migrations**: Django-style migrations with auto-detection
- **Authentication**: User management, sessions, and permissions
- **Form Validation**: Django-like form generation and validation
- **URL Routing**: Pattern-based routing with middleware support

## Try the Admin Interface

Run the blog admin example to see the admin interface in action:

```bash
cargo run -p corrode-admin --example blog_admin
```

Then open http://localhost:3000/admin/ and login with `admin` / `admin123`.

## Installation

Add the crates you need to your `Cargo.toml`:

```toml
[dependencies]
corrode-orm = "0.1"
corrode-admin = "0.1"
corrode-auth = "0.1"
corrode-forms = "0.1"
corrode-router = "0.1"
corrode-migrate = "0.1"
```

## Crates

- **corrode-router**: URL routing with middleware support
- **corrode-orm**: Django-like ORM with QuerySet, Manager, and Model
- **corrode-forms**: Form generation and validation with Bootstrap 5
- **corrode-migrate**: Database migrations with auto-detection
- **corrode-auth**: Authentication, sessions, and permissions
- **corrode-admin**: Django-like admin interface

## Development

```bash
make build          # Build the project
make test           # Run tests
make lint           # Run clippy
make format         # Format code
make example-blog   # Run blog admin example
make e2e-install    # Install E2E test dependencies
make e2e-test       # Run E2E tests
```

## License

MIT
