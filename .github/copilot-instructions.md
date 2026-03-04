# 🤖 GitHub Copilot Instructions for logue / logue向け GitHub Copilot 指示書

Please follow these specific coding standards based on the context.

## 🧱 General Formatting & Naming / 一般フォーマットと命名

- **Indent / インデント:** Use 2 spaces by default.
  - **Exceptions / 例外:** Use 4 spaces for **PHP** and **Rust**.
- **File Naming / ファイル命名:** Follow language/framework conventions for filenames.
  - **Vue:** Use **PascalCase** by default.
  - **Nuxt:** In directories where Nuxt conventions apply, use **kebab-case** (e.g. `pages`, `layouts`, `middleware`, `server/api`).
- **Variable Naming / 変数命名:** Use **camelCase**.
- **Type Naming / 型命名:** Use **PascalCase** for classes, interfaces, and structs.

## 🌐 Modern Web Stack (Primary) / モダンWebスタック（主軸）

- **Frontend & Backend / フロントエンド・バックエンド:** Use **Nuxt 3** (Nitro engine).
- **Vue System / Vue構成:** Use **Vue 3 (Composition API with <script setup>)**.
- **UI Framework Selection / UIフレームワーク選定:**
  - For rich/complex interfaces, use **Vuetify 3**.
  - Otherwise, use **Bootstrap 5**.
- **Tooling / ツール群:** Ensure compatibility with **ESLint**, **Prettier**, and **stylelint**.

## 🖥️ Desktop Development / デスクトップ開発

- **Standard / 標準構成:** **Tauri + Vuetify 3**.
- **Logic / ロジック:** Use idiomatic **Rust** (4-space indent).

## 🧩 Legacy / Occasional Maintenance / レガシー・保守対応

- **PHP / PHP:** Use **Laravel** or **Lumen**. Follow **Laravel Pint** standards.
- **Java / Java:** Use **Spring Boot** with **ActiveJDBC**. Follow **Google Java Styleguide**.
- **C# / C#:** Adhere to **stylecop.json**.

## 🎯 Active Focus / 現在の注力領域

- Prioritize development for **umd-core** and **tauri-vuetify-starter**.

## 🔒 Security / セキュリティ

- If you discover a security vulnerability, please **do not open a public issue**.
- Instead, please report it via one of the following:
  - **Email / メール:** <logue@hotmail.co.jp>
  - **GitHub Private Reporting / GitHub非公開報告:** Use the "Report a vulnerability" button in the Security tab if available.
- I will try to respond as soon as possible.

## 📚 Documentation / ドキュメント

- Use **Markdown** for all documentation.
- The documentation is in English and Japanese.
- Follow standard Markdown conventions for formatting and structure.
- Ensure documentation is clear, concise, and up-to-date with the latest code changes.
- For code snippets in documentation, use appropriate syntax highlighting for the language being demonstrated.
- Regularly review and update documentation to reflect any changes in code or project structure.
- Consider using tools like **Docusaurus** or **GitHub Pages** for hosting project documentation if it becomes extensive.
- Encourage contributions to documentation from the community, ensuring that it remains comprehensive and helpful for users of all levels.
- For security-related documentation, ensure that it is clear on how to report vulnerabilities and the expected response time.
- However, this may change to [Universal Markdown](https://github.com/logue/umd-core) syntax.

## 🗺️ Development Workflow / 開発ワークフロー

- At the current stage, use AI discussion to refine and consolidate requirements first.
- Write the consolidated draft specification in the repository root `PLAN.md`.
- After the specification is finalized, reflect the confirmed content in `docs` files and `README.md`.
- Keep `PLAN.md` as the working specification hub during implementation.

## Licensing / ライセンス

- All new projects and files should default to the **MIT License**.
- When generating a new project structure, ensure a `LICENSE` file is included.
