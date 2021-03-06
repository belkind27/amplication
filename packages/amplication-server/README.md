# Amplication Server

### Development

#### One time set up

- Make sure you have Node.js and Docker installed
- Install dependencies of the monorepo (execute in root directory):
  ```
  npm install
  npm run bootstrap
  ```
- Update code generated by Prisma
  ```
  npm run prisma:generate
  ```
- Update other generated code
  ```
  npm run generate
  ```
- Build all packages
  ```
  npm run build
  ```
- Get database services up (execute in server directory "packages/amplication-server")
  ```
  npm run docker:db
  ```
- Update application database (execute in server directory "packages/amplication-server")
  ```
  npm run start:db
  ```

#### Workflow

- Start the development server and watch for changes
  ```
  npm run start:watch
  ```
- Format files (editors like VSCode can do it for you automatically)
  ```
  npm run format
  ```
- Lint files (editors like VSCode come with integration to display those continuously)
  ```
  npm run lint
  ```
- Run tests and watch for changes
  ```
  npm run test:watch
  ```
- When needed, update Prisma Schema
  ```
  npm run migrate:save
  npm run migrate:up
  npm run prisma:generate
  ```
