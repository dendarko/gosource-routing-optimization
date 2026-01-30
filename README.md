  # GoSource Routing Optimization

GoSource Routing Optimization is a proof-of-concept system that computes optimal vehicle routes among suppliers to minimize transportation costs while meeting product demand and vehicle capacity constraints. It provides command-line tools for defining sourcing problems, building graph representations, and solving routes using Google OR Tools.

## Features

- **Data & CLI Tools**: Parse JSON input files that define suppliers, vehicles and demand; build graph representations and output optimal routes in JSON format.
- **Route Optimisation**: Utilises Google OR‑Tools and custom heuristics to determine cost‑efficient routes for product sourcing.
- **Quality Assurance**: Includes scripts to validate route solutions and ensure constraints (capacity, supply, demand) are satisfied.
- **Notifications & Integration**: Sends Slack notifications during pipeline execution and logs progress for monitoring.
- **Containerised & Reproducible**: Comes with Dockerfiles and CI/CD pipelines for reproducible builds and deployments.
- **Documentation**: Provides documentation and examples to help users understand the problem formulation and run the optimisation.

## Usage

```bash
# Solve a routing problem from an input JSON file
python -m gosource --input ./inputs/example_problem.json --output ./outputs/solution.json

# Run quality assurance checks on a solution
python -m gosource.qa --input ./outputs/solution.json
```

## Results

This proof‑of‑concept demonstrates how advanced algorithms can drastically reduce transportation costs and improve sourcing efficiency. The flexible framework can be adapted to a variety of logistics optimisation scenarios.
