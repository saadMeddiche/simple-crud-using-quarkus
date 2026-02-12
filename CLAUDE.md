# Project: Quarkus Fullstack (Qute + Web Bundler)

## 🛠 Tech Stack
- **Backend:** Quarkus 3+, Java 25, Hibernate Panache (Active Record pattern)
- **Frontend:** Qute Templates + Web Bundler (TypeScript/SCSS)
- **Database:** PostgreSQL

## 📏 Coding Standards
- **UI Modularity:** Always favor Qute Fragments and Tags over large monolithic templates to minimize context bloat.
- **Entities:** Use `PanacheEntity` for simple CRUD; `PanacheRepository` only if logic is complex.
- **Qute:** Keep logic in Java `@CheckedTemplate` or Controllers. Avoid complex JS logic inside `.html` files.
- **Bundler:** Place TS/JS in `src/main/resources/web/app/`. Don't manually edit `web/public/`.
- **Formatting:** Use standard Java/Google style. Prefer `var` for local variables.

## 📂 Navigation & Skills
- **UI/Bundler:** If working on styling/TS, call the `web-bundler` skill.

## 🚀 Common Commands
- **Dev Mode:** `./mvnw quarkus:dev`
- **Build Build:** `./mvnw package`
- **Clean Build:** `./mvnw clean package -DskipTests`
- **Tests:** `./mvnw test`