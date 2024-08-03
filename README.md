## Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

## Setup

1. **Clone the repository:**

    ```sh
    git clone https://github.com/yourusername/instagram-auto-poster.git
    cd instagram-auto-poster
    ```

2. **Install dependencies in the terminal:**

    ```sh
    npm install tough-cookie-filestore2
    npm install
    ```

3. **Environment Variables:**

    Create a `.env` file in the root directory and add the following environment variables:

    ```env
    PORT=4000
    INSTAGRAM_USERNAME=your_instagram_username
    INSTAGRAM_PASSWORD=your_instagram_password
    CONTENTFUL_SPACE_ID=your_contentful_space_id
    CONTENTFUL_ACCESS_TOKEN=your_contentful_access_token
    CONTENTFUL_MANAGEMENT_TOKEN=your_contentful_management_token
    INKY_DOODLE_EMAIL=your_email
    INKY_DOODLE_EMAIL_PASSWORD=your_email_password
    ```

## Usage

To start the application, run:

```sh
npm start
```

To terminate the application, run:

```sh
^c
```

The application will start and listen on the port specified in the `.env` file (default is 4000). The cron job will run every day at 4:00 PM and post a new Inky Doodle to Instagram.

## Libraries

- express
- axios
- contentful-management
- fs
- jimp
- instagram-web-api
- tough-cookie-filestore2
- node-cron
- imap-simple
- lodash
- mailparser
- dayjs
- dotenv

4. **Replace Data:**

    We need to replace all the example inkyDoodle data with our own data that we want to post.