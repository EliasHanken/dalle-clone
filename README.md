# Dall-E Clone

A clone of OpenAI's Dall-E, the state-of-the-art deep learning model for generating original images from textual descriptions.

## Prerequisites

- [Node.js](https://nodejs.org/en/download/)
- [MongoDB](https://docs.mongodb.com/manual/installation/)
- [Cloudinary account](https://cloudinary.com/signup)

## Technology Stack

- [Vite](https://github.com/vitejs/vite)
- JavaScript
- [MongoDB](https://www.mongodb.com/) for storage with [Express](https://expressjs.com/)
- [Cloudinary](https://cloudinary.com/) for image storage

## Installation

1. Clone the repository

```
git clone https://github.com/Streafe/dalle-clone.git
```

2. Navigate to the project directory

```
cd dalle-clone
```

3. Install dependencies

```
npm install
```

4. Create a `.env` file in the root directory with the following variables:

```
OPENAI_API_KEY=[YOUR_OPENAI_API_KEY]
MONGODB_URL=[YOUR_MONGODB_URL]

CLOUDINARY_CLOUD_NAME=[YOUR_CLOUDINARY_CLOUD_NAME]
CLOUDINARY_API_KEY=[YOUR_CLOUDINARY_API_KEY]
CLOUDINARY_API_SECRET=[YOUR_CLOUDINARY_API_SECRET]
```

5. Start the application

```
npm start
```

## Usage

- To generate an original image, make a `POST` request to `http://localhost:8080/api/v1/dalle` with the following JSON payload:

```
{
"prompt": "A three-story yellow house with a white picket fence and a red door."
}
```

- The response will contain the URL of the generated image, which is stored in the database and hosted on Cloudinary for better scalability.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
