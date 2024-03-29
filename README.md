
# Project Title

Dev Detective is a web application utilizing HTML, CSS, and JavaScript to enable users to search for GitHub usernames. Upon input, it fetches basic user data from the GitHub API, displaying information such as repositories, followers, and bio. The interface offers a seamless experience with optional light and dark mode themes.

# Project Demo
https://soumyadeori.github.io/Dev-Detective/

# Project Structure
```bash
📦 Dev-Detective
 ┣ 📂 assets
 ┃ ┣ 📂 images
 ┃ ┃ ┣ 📜 apple-touch-icon.png
 ┃ ┃ ┣ 📜 favicon-16x16.png
 ┃ ┃ ┗ 📜 favicon-32x32.png
 ┃ ┗ 📜 site.webmanifest
 ┣ 📜 index.html
 ┣ 📜 styles.css
 ┣ 📜 script.js
 ┗ 📜 README.md
 ```

# GitHub API Reference

## Get User Information

Retrieves information about a GitHub user.

### HTTP Request

GET https://api.github.com/users/{username}


### Parameters

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `username`| `string` | **Required**. GitHub username |

### Response

The API returns JSON data with the following fields:

| Field              | Type     | Description                              |
| :----------------- | :------- | :--------------------------------------- |
| `login`            | `string` | GitHub username                          |
| `name`             | `string` | Full name of the user                    |
| `avatar_url`       | `string` | URL of the user's avatar image           |
| `bio`              | `string` | Biography of the user                    |
| `public_repos`     | `number` | Number of public repositories            |
| `followers`        | `number` | Number of followers                      |
| `following`        | `number` | Number of users followed                 |
| `location`         | `string` | Location of the user                     |
| `blog`             | `string` | URL of the user's website                |
| `twitter_username` | `string` | Twitter handle of the user               |
| `company`          | `string` | Company the user is associated with      |
