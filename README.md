# Slide Share Research Agent Flow

This project contains a declarative CrewAI Flow exported from CrewAI Studio.

The main flow definition is located at:

`src/slide_share_research_agent/flow.json`

## What It Does

The prototype is designed as a reusable AI research automation workflow that:

- Accepts natural-language research queries
- Generates research queries
- Searches and collects accessible web content
- Extracts structured information
- Validates and filters results
- Removes duplicates
- Maintains checkpoint and progress information
- Produces structured output and a summary report

## Current Prototype Status

The complete workflow has been built and tested end-to-end in CrewAI Studio.

The current limitation is the SlideShare source-access layer. SlideShare's search pages are heavily JavaScript-rendered, and the available automated search route currently does not provide usable results without additional external access/API availability.

The workflow is therefore designed so the source-access method can be replaced or connected to an authorized access method without rebuilding the rest of the pipeline.

## Project Structure

```text
src/
└── slide_share_research_agent/
    ├── __init__.py
    └── flow.json
