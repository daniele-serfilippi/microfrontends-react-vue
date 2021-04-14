# Simple Microfrontends Architecture

Using Webpack Module Federation to create a microfrontends architecture with 4 sub-projects:

- Container (React)
- Marketing (React)
- Auth (React)
- Dashboard (Vue)

To run it, run each of this command in a different shell:
```
npm --prefix ./packages/container install && npm --prefix ./packages/container start
npm --prefix ./packages/marketing install && npm --prefix ./packages/marketing start
npm --prefix ./packages/auth install && npm --prefix ./packages/auth start
npm --prefix ./packages/dashboard install && npm --prefix ./packages/dashboard start
```

The whole application will run on:
```
http://localhost:8080
```

The 3 microfrontends sub-projects will also run in isolation on:
```
http://localhost:8081 (Marketing)
http://localhost:8082 (Auth)
http://localhost:8083 (Dashboard)
```
