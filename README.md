# Calendar MCP Server

A Model Context Protocol (MCP) server that provides access to Google Calendar data through a simple API.

## Description

This MCP server allows you to retrieve calendar events for a specific date using Google Calendar API integration. It's built with Node.js and the MCP SDK.

## Features

- Retrieve calendar events for a specific date
- Google Calendar API integration
- MCP-compatible tool interface

## Prerequisites

- Node.js (version 14 or higher)
- Google Calendar API credentials
- A Google Calendar ID

## Installation

1. Clone or download this repository
2. Install dependencies:
   ```bash
   npm install
   ```

## Configuration

1. Create a `.env` file in the root directory
2. Add your Google API credentials:
   ```
   GOOGLE_PUBLIC_API_KEY=your_google_api_key_here
   CALENDAR_ID=your_calendar_id_here
   ```

## Usage

### Starting the Server

```bash
npm start
```

### Using the Tool

The server provides a tool called `getMyCalendarDataByDate` that accepts a date parameter and returns calendar events for that date.

**Parameters:**
- `date`: A valid date string (e.g., "2024-01-15")

**Returns:**
- JSON object containing meetings/events for the specified date

## Dependencies

- `@modelcontextprotocol/sdk`: MCP SDK for server implementation
- `dotenv`: Environment variable management
- `googleapis`: Google APIs client library
- `zod`: Schema validation

## License

ISC

## Author

Nahid 