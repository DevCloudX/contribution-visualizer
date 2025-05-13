# GitHub Contribution Snake

This repository generates a unique animated snake game based on the contribution graph of a GitHub user. The snake's movement is determined by the contributions made by the user, creating an engaging and visual representation of their activity on GitHub.

## Features

- Generates an SVG animation from a GitHub user's contribution graph.
- Creates two versions of the animation: one for the light theme and one for the dark theme.
- Automatically pushes the generated SVG animation to a specified `output` branch.
- Can be viewed through a raw GitHub URL or hosted via GitHub Pages.

## How It Works

1. The workflow is triggered when a push is made to the `main` branch or manually via the GitHub Actions UI.
2. It fetches the contribution graph of the repository owner.
3. It generates an SVG animation of the GitHub contribution graph using the **Platane/snk** GitHub Action.
4. The animation is then pushed to a designated `output` branch of the repository.
5. The animation can be accessed directly via a GitHub raw URL or viewed via GitHub Pages.

## Usage

1. **Fork the repository** to your own GitHub account.
2. Ensure you have the necessary permissions to push to the `output` branch.
3. Trigger the workflow either by:
   - Pushing to the `main` branch.
   - Manually triggering it via the GitHub Actions UI under the "Actions" tab.

Once the workflow completes, the generated SVG files will be available in the `output` branch.

## Example Output

- [GitHub Contribution Snake (Light Theme)](https://raw.githubusercontent.com/<username>/<repo>/output/dist/github-contribution-grid-snake.svg)
- [GitHub Contribution Snake (Dark Theme)](https://raw.githubusercontent.com/<username>/<repo>/output/dist/github-contribution-grid-snake-dark.svg?palette=github-dark)

## Contributing

Feel free to fork the repository, improve the workflow, or create issues for any bugs or enhancements. Pull requests are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
