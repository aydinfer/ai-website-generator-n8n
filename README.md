# AI Website Generator - n8n Workflow

This repository contains n8n workflows for an AI-powered website generation system. The system uses different agent types (Planner, Content, Designer, WordPress) and includes components like a memory system, orchestrator, and error handling.

## Setup Instructions

1. **Install n8n**
   ```
   npm install n8n -g
   ```

2. **Start n8n**
   ```
   n8n start
   ```

3. **Import Workflows**
   - Open n8n in your browser (default: http://localhost:5678)
   - Go to Workflows > Import from File/URL
   - Import the workflow files from the `workflows` directory

4. **Configure Credentials**
   - Set up API credentials for any external services used

## Components

### Memory System
Stores and retrieves context between workflow runs using vector embeddings for semantic search.

### Orchestrator
Manages the workflow sequence and coordinates between different agent types.

### Agent Workflows
- **Planner Agent**: Creates the overall plan for the website
- **Content Agent**: Generates content based on the plan
- **Designer Agent**: Creates design elements
- **WordPress Agent**: Deploys the website to WordPress

### Error Handling
Implements retry mechanisms, checkpointing, and notifications for failures.

## Usage

1. Trigger the main workflow using the webhook URL
2. Monitor the workflow through the n8n dashboard
3. Check logs for detailed information about each step

## Contributing

Feel free to submit issues or pull requests to improve the workflows.
