# Facebook Comments Scraper (Free Limited Version)

This tool scrapes up to **100 main comments** from a public Facebook post, share link, or reel. Results are exported to an Excel file.

> **Note:** This free version does **not** include replies or unlimited comments.  
> If you need unlimited comments and replies, contact me for a one-time premium fee.

## Features

- Fast extraction using Facebook's GraphQL API (works 99% of the time).
- Extracts up to 100 main comments from Facebook posts, share links, and reels.
- Follows share link redirects automatically.
- Encodes post IDs for Facebook's GraphQL API.
- Handles Facebook token rotation to mitigate blocking by Facebook's anti-bot system.
- Exports results to Excel with metadata.

## Usage

```bash
go run main.go <facebook_post_url_or_share_link>
```

### Examples

- Scrape from a share link:
  ```
  go run main.go "https://web.facebook.com/share/p/1AguUnrRzz/"
  ```
- Scrape from a direct post URL:
  ```
  go run main.go "https://web.facebook.com/username/posts/pfbid123..."
  ```
- Scrape from a base64 encoded post ID (advanced):
  ```
  go run main.go "ZmVlZGJhY2s6cGZiaWQxMjM..."
  ```

## Output

- Comments are exported to an Excel file in the `exports/` directory.
- Excel columns: Comment ID, Author Name, Author ID, Comment Text, Created Time, Likes Count, Reply Count, Depth, Is Reply, Parent Comment

## Requirements

- Latest Go version
- Internet connection
- Public Facebook post URL or share link

## Support

- **Free installation support** is available if you get stuck—just reach out!

## Premium Version

- Need unlimited comments and replies?  
  Contact me for a one-time premium fee.

## Contact

- **Email:** haronkibetrutoh@gmail.com
- **WhatsApp:** +254718448461
