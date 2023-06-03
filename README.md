# Caption Generator API

This repository contains the code for a Caption Generator API that utilizes the Django REST Framework, the nlpconnect/vit-gpt2-image-captioning pretrained model, and the OpenAI API to generate captions for Instagram posts.
## Endpoint

The backend exposes a single endpoint:

### `/caption_generator`

This endpoint accepts a POST request and returns a JSON response containing the caption for the provided image.

**Request Parameters:**

- `img_link` (string): The link to the image to be processed.

**Example Request:**

```json
{
  "img_url": "image/url"
}
```

**Example Response:**

```json
{
  "caption": "Chasing My Dreams ⚽️🏃‍♂️"
}
```

## Setup

To set up the Caption Generator backend locally, follow the instructions below:

1. Clone the repository:

   ```bash
   git clone https://github.com/mbahraoui/https://github.com/mbahraoui/CaptionGeneratorAPI.git
   ```
   

2. Navigate to the project directory:

   ```bash
   cd CaptionGeneratorAPI
   ```

3. Create a `.env` file in CaptionGenerator directory of the project and add the following line:

   ```plaintext
   API_KEY=your_api_key
   ```

   Replace `your_api_key` with your actual GPT-3 API key.

4. Start the Django development server:

   ```bash
   python manage.py runserver
   ```

   The backend should now be running at `http://localhost:8000/`.
.
