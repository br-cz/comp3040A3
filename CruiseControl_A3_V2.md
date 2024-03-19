# API Documentation

Change title??

### Description

The RandomProfileImage API is designed to provide developers a seamless experience for generating a default profile picture for users who do not wish to upload a picture upon account creation. It offers a simple and intuitive interface for developers that will allow them to easily integrate it into their applications.

### Resources

The API provides access to random images related to cryptocurrency/blockchain technology. Each image resource is represented as a JSON object with the following attributes:

```json
{
  "id": "1",
  "url": "https://example.com/random-image.jpg",
  "category": "bitcoin",
  "type": "jpg",
  "color": "red"
}
```

Where:

- `id`: The unique identifier of the image.
- `url`: The URL of the image.
- `category`: The category of the image (e.g., 'bitcoin', 'ethereum', 'blockchain').
- `type`: The type of the image (e.g., 'jpg', 'png', 'gif').
- `color`: The color schema used in the image (e.g., a blue bitcoin).

### Endpoint

1. **Get Random Image**
   - Endpoint: `/random-image`
   - Method: `GET`
   - Parameters:
     - `category` (optional): Specifies the category of the random image (e.g., 'bitcoin', 'ethereum', 'blockchain'). If not provided, images from all categories will be considered.
     - `type` (optional): Specifies the type of the random image (e.g., 'jpg', 'png', 'gif'). If not provided, any image type will be considered.
     - `color` (optional): Specifies the color of the random image (e.g., 'jpg', 'png', 'gif'). If not provided, any image color will be considered.

#### Sample Request with Sample Response

##### Request:

`GET /random-image?category=bitcoin&type=jpg`

##### Response:

```json
{
  "id": "1",
  "url": "https://example.com/random-bitcoin-image.jpg",
  "category": "bitcoin",
  "type": "jpg"
}
```
