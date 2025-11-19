# Osisi Frontend

This is the frontend repository for the **Osisi** project. It is built to provide a user-friendly interface for interacting with the Osisi platform.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [License](#license)

## Features

- Responsive design for various devices.
- Seamless integration with the backend API.
- User authentication and authorization.
- Dynamic content rendering.

## Technologies Used

- **Framework**: Next.js
- **State Management**: Zustand
- **Styling**: CSS and Tailwind
- **Build Tool**: Webpack
- **Package Manager**: npm
- **Backend**: Convex
- **Canvas**: React flow
- **Authentication**: Auth0 (we are moving to better auth)

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm

### Contributing

We follow the Fork & Pull Request workflow for contributions. Here's how you can contribute:

### Step 1: Set Up Your Environment

1. **Fork the Repository**:

   - Visit the main repository at `https://github.com/Hemephelus/CSC-419-CLASS-PROJECT`
   - Click the "Fork" button in the top right corner to create your own copy

2. **Clone Your Fork**:

   ```bash
   git clone https://github.com/Hemephelus/CSC-419-CLASS-PROJECT.git
   cd CSC-419-CLASS-PROJECT
   ```

3. **Add the Upstream Remote**:
   ```bash
   git remote add upstream https://github.com/Hemephelus/CSC-419-CLASS-PROJECT.git
   ```

### Step 2: Create a Feature Branch

1. **Sync with the Upstream Repository**:

   ```bash
   git fetch upstream
   git checkout main
   git merge upstream/main
   ```

2. **Create a New Branch**:
   ```bash
   git checkout -b feature/your-feature-name
   ```
   Use a descriptive name for your branch (e.g., `feature/added-comments` or `fix/date-issue`)

### Step 3: Make Your Changes

1. **Implement Your Feature or Fix**:

   - Write clean, well-documented code
   - Include comments where necessary

2. **Commit Your Changes**:
   ```bash
   git add .
   git commit -m "Add meaningful commit message describing your changes"
   ```
   Write clear, concise commit messages that explain what your changes do

### Step 4: Submit a Pull Request

1. **Push Your Changes to Your Fork**:

   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create a Pull Request**:

   - Go to your fork on GitHub
   - Click the "Compare & pull request" button for your branch
   - Provide a clear description of your changes
   - Reference any relevant issues using the # symbol (e.g., "Fixes #42")

3. **Wait for Review**:
   - Project maintainers will review your PR
   - Be responsive to any feedback or requests for changes
   - Make additional commits to your branch if needed

### Step 5: After Your PR is Merged

1. **Sync Your Fork**:
   ```bash
   git checkout main
   git fetch upstream
   git merge upstream/main
   git push origin main
   ```

### Running the Application

To start the web development server:

```bash
npm run start
```

The application will be available at `http://localhost:3000`.

To start the convex development server:

```bash
npx convex dev --env-file .env.development
```

Note ask nwachukwu for the .env files

### Building for Production

To create a production build:

```bash
npm run build
```

## Folder Structure

```
osisi/
├── .vscode/
├── convex/
│   ├── _generated/
│   ├── authorization/
│   ├── collaborators/
│   ├── families/
│   ├── familyMembers/
│   ├── relationships/
│   ├── users/
│   ├── auth.config.ts
│   ├── convex.config.ts
│   ├── migrations.ts
│   ├── README.md
│   ├── schema.ts
│   └── tsconfig.json
├── public/
├── src/
│   ├── app/
│   ├── components/
│   ├── contexts/
│   ├── features/
│   ├── fullstack/
│   ├── hooks/
│   ├── lib/
│   ├── sketches/
│   ├── utils/
│   ├── middleware.ts
│   └── types.ts
├── .gitignore
├── components.json
├── eslint.config.mjs
├── next.config.ts
├── package-lock.json
├── package.json
├── postcss.config.mjs
├── README.md
├── tsconfig.json
└── vitest.config.mts
```
