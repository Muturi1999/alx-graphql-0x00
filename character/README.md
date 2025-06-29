markdown# GraphQL Character Queries by ID and Pagination

This project demonstrates how to query specific characters using their ID and retrieve paginated lists of characters from a GraphQL API.

## Project Structure
alx-graphql-0x00/
└── character/
├── README.md
├── character-id-1.graphql
├── character-id-1-output.json
├── character-id-2.graphql
├── character-id-2-output.json
├── character-id-3.graphql
├── character-id-3-output.json
├── character-id-4.graphql
├── character-id-4-output.json
├── characters-page-1.graphql
├── characters-page-1-output.json
├── characters-page-2.graphql
├── characters-page-2-output.json
├── characters-page-3.graphql
├── characters-page-3-output.json
├── characters-page-4.graphql
└── characters-page-4-output.json

## Query Types

### 1. Individual Character Queries
Query specific characters by their ID using the `character(id: ID!)` field.

**Fields Retrieved:**
- `id` - The unique identifier of the character
- `name` - The character's name
- `status` - Whether the character is Alive, Dead, or Unknown
- `species` - The species of the character
- `type` - Additional type information
- `gender` - The character's gender

### 2. Paginated Characters Queries
Query paginated lists of characters using the `characters(page: Int)` field.

**Fields Retrieved:**
- `id` - The unique identifier of the character
- `name` - The character's name
- `status` - Whether the character is Alive, Dead, or Unknown
- `image` - URL to the character's image

**Pagination Info:**
- `count` - Total number of characters
- `pages` - Total number of pages
- `next` - Next page number (if available)
- `prev` - Previous page number (if available)

## How to Use

1. Execute each GraphQL query against your GraphQL endpoint
2. Save the responses in the corresponding output JSON files
3. Use the pagination info to navigate between pages

