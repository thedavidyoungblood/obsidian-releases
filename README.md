## About this repo

This repo is used for hosting public releases of Obsidian, as well as our community plugins & themes directories.

Obsidian is not open source software and this repo _DOES NOT_ contain the source code of Obsidian. However, if you wish to contribute to Obsidian, you can easily do so with our extensive plugin system. A plugin guide can be found here: https://docs.obsidian.md

This repo does not accept issues, if you have questions or issues with plugins, please go to their own repo to file them. If you have questions or issues about core Obsidian itself, please post them to our community: https://obsidian.md/community

## Submit your plugin or theme

When opening a pull request, please switch to preview mode and select the option to go through our submission checklist. Submit your entry by following the convention in the JSON file and we will review your submission.

Thanks for submitting your creations!

You can find a detailed explanation for submitting your [plugin here](https://docs.obsidian.md/Plugins/Releasing/Submit+your+plugin) and your [theme here](https://docs.obsidian.md/Themes/App+themes/Submit+your+theme).

## Policies

All submissions must conform with our [developer policies](https://docs.obsidian.md/Developer+policies)

## Community Theme

To add your theme to our theme store, make a pull request to the `community-css-theme.json` file. Please add your theme to the end of the list.

- `name`: a unique name for your theme. Must not collide with other themes.
- `author`: the author's name for display.
- `repo`: the GitHub repository identifier, in the form of `user-name/repo-name`, if your GitHub repo is located at `https://github.com/user-name/repo-name`.
- `screenshot`: path to the screenshot of your theme.
- `modes`: if your theme supports both dark and light mode, put `["dark", "light"]`. Otherwise, put `["dark"]` if your theme only supports dark mode, or  `["light"]` if your theme only supports light mode.
- `publish`: if your theme supports Obsidian Publish, set this to `true`. Omit it otherwise.

To get your theme compatible with Obsidian Publish, you can use `applyCss` and `applyCssByLink` to test out your CSS in the developer console of Obsidian Publish sites, so that you don't actually need to own sites to test your `publish.css`. You can test it out on our help site here: https://help.obsidian.md/

`applyCss` takes a CSS string, you can use backtick (template strings) for multiline CSS. `applyCssByLink` takes a link and loads the CSS, would recommend GitHub raw file URLs.

## Community Plugin

### Community Plugins format

To add your plugin to the list, make a pull request to the `community-plugins.json` file. Please add your plugin to the end of the list.

- `id`: A unique ID for your plugin. Make sure this is the same one you have in your `manifest.json`.
- `name`: The name of your plugin.
- `author`: The author's name.
- `description`: A short description of what your plugin does.
- `repo`: The GitHub repository identifier, in the form of `user-name/repo-name`, if your GitHub repo is located at `https://github.com/user-name/repo-name`.

### How community plugins are pulled

- Obsidian will read the list of plugins in `community-plugins.json`.
- The `name`, `author` and `description` fields are used for searching.
- When the user opens the detail page of your plugin, Obsidian will pull the `manifest.json` and `README.md` from your GitHub repo).
- The `manifest.json` in your repo will only be used to figure out the latest version. Actual files are fetched from your GitHub releases.
- If your `manifest.json` requires a version of Obsidian that's higher than the running app, your `versions.json` will be consulted to find the latest version of your plugin that is compatible.
- When the user chooses to install your plugin, Obsidian will look for your GitHub releases tagged identically to the version inside `manifest.json`.
- Obsidian will download `manifest.json`, `main.js`, and `styles.css` (if available), and store them in the proper location inside the vault.

### Announcing the First Public Release of your Plugin/Theme

- Once admitted to the plugin/theme browser, you can announce the public availability of your plugin/theme:
  - [in the forums](https://forum.obsidian.md/c/share-showcase/9) as a showcase, and
  - [on the Discord Server](https://discord.gg/veuWUTm) in the channel `#updates`. (You need the `developer` role to be able to post in that channel; [you can get that role here](https://discord.com/channels/686053708261228577/702717892533157999/830492034807758859).)
- You can also announce the first working version of your plugin as a public beta before "officially" submitting it to the plugin/theme browser. That way, you can acquire some beta testers for feedback. It's recommended to use the [BRAT Plugin](https://obsidian.md/plugins?id=obsidian42-brat) to make the installation as easy as possible for interested beta testers.

## Data Governance Compliance and Continuous Monitoring Tools

To ensure data governance compliance and continuous monitoring for new plugins and themes, please follow these guidelines:

- **Data Governance Compliance**: Ensure that your plugin or theme adheres to data governance policies. This includes implementing tools for continuous data quality monitoring and conducting regular audits to ensure compliance with data governance policies.
- **Continuous Monitoring Tools**: Implement continuous monitoring tools to ensure real-time system oversight. Configure alerts for critical issues to ensure timely response and resolution.

## New Developer Repository Ramp-Up Guide

For a comprehensive guide to understanding and mastering this repository, please refer to the [New Developer Repository Ramp-Up Guide](./New-Dev-REPO-RAMP-UP-GUIDE.md). This guide includes detailed instructions on setting up the development environment, understanding the code structure, and contributing to the repository.

## ABSOLUTE-ULTIMATE Ægentic Project Management Entity (AUÆPME)

### Role and Capabilities

The AUÆPME is designed to orchestrate, choreograph, and manage all aspects of project creation, design, development, implementation, administration, adaptive-dynamic evolution, and concurrent management with unparalleled precision and efficiency.

### Project Lifecycle Phases Managed by AUÆPME

- **Assessment Phase**:
  - Current Systems Evaluation
  - Requirements Gathering
  - Gap Analysis
- **Design Phase**:
  - Architectural Planning
  - Tool Selection
  - Workflow Blueprinting
  - Data Governance Planning
- **Development Phase**:
  - Automation Script Development
  - Integration Setup
  - Module Construction
  - Data Governance Implementation
  - Data Quality Tools Setup
- **Testing Phase**:
  - Unit Testing
  - Integration Testing
  - Security Testing
  - Performance Testing
  - Data Quality Testing
- **Deployment Phase**:
  - Staging Environment Setup
  - Production Rollout
  - Monitoring Setup
- **Maintenance Phase**:
  - Regular Updates
  - Continuous Monitoring
  - Feedback Integration
  - Data Governance Audits

### Development Paradigms and Principles Integrated by AUÆPME

- **Agile Methodology**: Implement iterative development cycles, fostering flexibility and responsiveness to change.
- **DevOps Practices**: Integrate development and operations for continuous delivery, automating deployment pipelines to enhance efficiency.
- **Continuous Integration/Continuous Deployment (CI/CD)**: Automate testing and deployment processes, ensuring rapid and reliable delivery of features and fixes.
- **Test-Driven Development (TDD)**: Write tests before developing functionality, ensuring code meets requirements and is maintainable.
- **SOLID Principles**:
  - Single Responsibility
  - Open/Closed
  - Liskov Substitution
  - Interface Segregation
  - Dependency Inversion
- **DRY (Don't Repeat Yourself)**: Eliminate duplication in code and processes, promoting reusability and maintainability.
- **KISS (Keep It Simple, Stupid)**: Simplify designs and implementations, avoiding unnecessary complexity.
- **YAGNI (You Aren't Gonna Need It)**: Implement features only when necessary, preventing overengineering.

### Paired-Qualities for Team Alignment and Accountability

- **Collaboration & Communication**: Foster open and transparent communication channels, encouraging collaborative problem-solving and decision-making.
- **Accountability & Responsibility**: Define clear roles and responsibilities for each team member, implementing accountability mechanisms to track progress and performance.
- **Adaptability & Flexibility**: Promote adaptability to changing project requirements, encouraging flexibility in approaches and solutions.
- **Continuous Learning & Improvement**: Support ongoing education and skill development, implementing feedback loops for continuous process enhancement.
- **Quality & Excellence**: Uphold high standards for all deliverables, striving for excellence in every aspect of the project.

### Visualization and Orchestration Tools Used by AUÆPME

- **Stage-Based Workflow Mapping**: Utilize stage/phase/layer-based visualizations to represent project workflows, highlighting interdependencies and orchestration without relying on chronological timelines.
- **Interoperable-Interdependencies**: Clearly depict how different project components interact and depend on each other, ensuring visual aids reflect the complexity and connectivity of the project structure.

#### Supplemental Visualizations

- **Mermaid Diagrams**:
  - Flow Diagram: Illustrate the overall workflow of the software development lifecycle.
  - Sequence Diagram: Depict interactions between different components over stages.
  - Mindmap: Represent the hierarchical structure of the development phases.
  - Class Diagram: Show the relationships between different classes/modules.
  - State Diagram: Outline the various states of the system throughout development.
  - ER Diagram: Map out the entity-relationship for data management.
  - Gantt Chart: Visualize project timelines using stage/phase-based structures.
  - Git Diagram: Display version control workflows and branching strategies.
  - User Journey: Illustrate the end-user interactions and experiences.
  - Quadrant Chart: Analyze aspects such as priority vs. effort.
  - XY Chart: Represent metrics and performance indicators.
  - Block Diagram: Show high-level system architecture and component interactions.
  - Packet Diagram: Detail data packet flows and communication protocols.
- **Python Library Visualizations**:
  - Utilize libraries such as Matplotlib, Seaborn, and Plotly to create advanced visual representations.
  - Generate interactive dashboards to monitor development metrics.
  - Create network graphs to illustrate component interdependencies.
  - Develop heatmaps for testing coverage and performance metrics.
  - Implement Sankey diagrams to represent data flows and integrations.
