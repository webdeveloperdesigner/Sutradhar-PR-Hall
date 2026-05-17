# 🏛️ Sutradhar Hall - Contributor Platform

Welcome to **Sutradhar Hall**, the official contributor recognition platform for the Sutradhar open-source ecosystem. This system is specifically designed to celebrate open-source contributions and empower beginners to confidently learn Git and GitHub pull request workflows.

Here, contributors can showcase their skills, contribution journey, active streak, and profile details by editing a single, safe contributor file.

---

## ✨ Features

- **🏆 Contributor Hall of Fame**: A dynamic, searchable leaderboard showcasing merged PRs, streak statistics, and developer ranks.
- **🎨 Interactive Profile Builder**: A visual wizard with step-by-step guidance that assists you in configuring your custom profile and selected bio archetypes.
- **⚙️ Dynamic JSON Compilation**: Automatic loading of user JSON profiles using dynamic module imports. Maintainers merge your PR, and your profile immediately appears on the live site!
- **⚡ Rate-Limit Resilient**: Embedded caching layers and safe **UI Avatars** initial fallbacks to bypass GitHub unauthenticated API rate limits.
- **💫 Premium Visual Systems**:
  - **Skiper31 3D Typography Scroll Animation**: Staggered scroll-driven parallax transitions revealing character letter components in 3D space.
  - **Skiper40 CSS Links**: Stylized, high-fidelity responsive hover link animations with smooth transitions.

---

## 🛠️ Technology Stack

- **Framework**: React.js & React Router
- **Animations**: Framer Motion (Scroll & Perspective transformations)
- **Icons**: Lucide React
- **Styling**: Plain, optimized CSS (Vanilla styling architecture)
- **Data Integration**: JSON-based profiles dynamically fetched and cached alongside the GitHub API.

---

## 🚀 How to Add Your Contributor Profile

Getting listed on the official Hall of Fame is super easy and 100% beginner-safe. Follow these simple steps:

### Step 1: Fork the Repository

Click the **Fork** button at the top-right of the GitHub repository to create a copy in your own GitHub account.

### Step 2: Use the Profile Builder Wizard

1. Run the project locally (see [Local Development](#-local-development)) or visit the live site.
2. Click **Create Profile** in the navigation bar to open the builder.
3. Fill in your details:
   - Your real GitHub username
   - A custom display name & role
   - A personalized bio (or select a premium pre-made **Developer Archetype**!)
   - Select your preferred theme color accent & skills tags
4. Once satisfied, click the **Copy JSON** button in the _Terminal Output Code Card_ on the right!

### Step 3: Create Your Profile File

In your forked repository, navigate to:

```bash
src/contributors/
```

Create a new file named exactly `[your-github-username].json` (e.g. `octocat.json`) and paste the copied JSON contents inside.

> [!IMPORTANT]  
> Only write/edit this single file! Do not modify any other codebase structures. This ensures your pull request is merged immediately and automatically.

### Step 4: Create a Pull Request (PR)

1. Commit your changes and push them to your fork.
2. On GitHub, click **New Pull Request**.
3. Submit your PR with a title like `feat: add [your-username] contributor profile`.
4. Once merged by our maintainers, the build compilation system will bundle your file and add you to the Hall of Fame automatically!

---

## 💻 Local Development

Follow these steps to run the application locally on your machine:

### Prerequisites

Ensure you have [Node.js](https://nodejs.org/) installed.

### Quick Start (Run Locally)

If you already have this repository on your local machine:

1. **Install dependencies**:

   ```bash
   npm install
   ```

2. **Start the development server**:

   ```bash
   npm start
   ```

   _The application will automatically open at [http://localhost:3000](http://localhost:3000)._

3. **Build for production**:
   ```bash
   npm run build
   ```

---

## 🛡️ Contribution Guidelines & Safety

To keep the platform safe and friendly for everyone:

- **Only edit your own file** under `src/contributors/[your-username].json`.
- **Do not include private information** like emails or passwords in your JSON.
- **Ensure JSON formatting is correct** (the builder ensures valid formatting automatically!).
- **Be respectful and kind** in your bio content.

Happy hacking, and welcome to the open-source community! 🚀

