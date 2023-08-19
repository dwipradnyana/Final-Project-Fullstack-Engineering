# GIGIH TOKOPEDIA PLAY

## Features

**1. Home Page** - Users can see a list of video thumbnails on the home page.

**2. Detail Video Page** - when visit a specific video page, users can see a list of associated products, and engage with the comments section.

**3. Comments interaction** - Users can read existing comments on video pages and post new comments.

**4. 404 Not Found Page** - If a user tries to access an unknown page, they will be redirected to a custom 404 page.

## Prerequisites

Before running the project, make sure you have the following software installed on your machine:

- [Node.js-V18](https://nodejs.org/)

## Installation

**1. Clone the Repository:** Use `git clone` to clone this repository to your local machine.

```
git clone https://github.com/Naufal-dzaki/GIGIH-TOKOPEDIA-PLAY.git
cd GIGIH-TOKOPEDIA-PLAY
```

**2. Install Dependencies:** Install the required dependencies using a package manager like npm or yarn.

```
npm install
```

**3. Run the App:** Start the development server to run the app locally.

```
npm start
```

**4. Access the App:** Open your web browser and navigate to `http://localhost:3000` to access the app.

## Schema Database

### A. Videos

**1. Videos's Collection Structure**

| Key       | Type     | Description                   |
| --------- | -------- | ----------------------------- |
| \_id      | ObjectId | unique identifier             |
| title     | String   | title for the video           |
| img_url   | String   | URL for the video's thumbnail |
| video_url | String   | URL for the video             |
| createdAt | date     | Auto generate by mongoDB      |
| updatedAt | date     | Auto generate by mongoDB      |

### B. Products

**1. products's Collection Structure**

| Key         | Type     | Description                          |
| ----------- | -------- | ------------------------------------ |
| \_id        | objectId | unique identifier                    |
| video_id    | objectId | video's collection unique identifier |
| product_url | String   | URL for the product link             |
| img_url     | String   | URL for the product image            |
| title       | String   | title for the product                |
| price       | Number   | price for the product                |
| createdAt   | date     | Auto generate by mongoDB             |
| updatedAt   | date     | Auto generate by mongoDB             |
