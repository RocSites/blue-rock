# Blue Rock Website and CMS

This repository contains the `frontend` (Gatsby) and `backend` (Strapi) for Blue Rock

To start the `backend`, navigate to the `/backend` folder and run `yarn develop`

-----

**NOTE** in order for the frontend to consume the backend API (GraphQL), you'll need to generate an API token and then add to that the `.env` file at the root of the `frontend`.

**To generate the API token follow these steps**: 
 
1. Start your backend (should be on `localhost:1337`)
2. Login to the admin (<a href="localhost:1337/admin">localhost:1337/admin</a>)
3. Navigate to Settings/Global Settings/API Tokens
4. Click on "Create new API Token"
5. SAVE that token somewhere, then paste it into your .env file as a the `STRAPI_TOKEN`

 
 Your `.env` file should look like this: 
```
STRAPI_TOKEN=putYourTokenHere
STRPI_API_URL=
```

To start the `frontend`, navigate to the `/frontend` and run `yarn start`. It'll be on `localhost:8000`
