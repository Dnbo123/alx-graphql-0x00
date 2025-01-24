# GraphQL Episode Query

This project contains a GraphQL query to retrieve details of an episode using the `episode(id: ID!)` field. The query fetches specific fields like `id`, `name`, `air_date`, and `episode` for a given episode ID.

## Query Description

The GraphQL query retrieves the following fields:
- **`id`**: The unique identifier of the episode.
- **`name`**: The name of the episode.
- **`air_date`**: The date the episode first aired.
- **`episode`**: The episode code (e.g., "S01E01").

### Example Query

```graphql
query GetEpisodeById {
  episode(id: 1) {
    id
    name
    air_date
    episode
  }
}
