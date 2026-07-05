# Expense Tracker MCP Server

An MCP server built with FastMCP and SQLite that integrates with Claude Desktop.

## Features

- Add expenses
- List expenses by date range
- Summarize spending by category
- Categories resource endpoint
- SQLite persistence

## Tools

### add_expense

Add a new expense entry.

### list_expenses

Retrieve expenses between two dates.

### summarize

Get spending totals grouped by category.

## Resource

expense://categories

## Run locally

```bash
uv sync
uv run python main.py
```

## Claude Desktop

Add to `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "ExpenseTracker": {
      "command": "python",
      "args": ["D:\\path\\to\\main.py"]
    }
  }
}
```

Built with FastMCP 🚀
