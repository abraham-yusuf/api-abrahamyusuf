# Web3ID API
## For Blog and NFT Marketplace

### Running locally

Create a folder and `git clone` from this repository.

Install the dependencies and start the dev server.

```bash
    yarn install
    yarn develop
```

The strapi server will run on [http://localhost:1337](http://localhost:1337)

Go to the admin panel [(http://localhost:1337/admin)](http://localhost:1337), create an account and start adding sample content.

### Deployment

First, you'll need a [Cloudinary](https://cloudinary.com) and a [Heroku](https://www.heroku.com/) account.

1. From your copy of the repo click the "Deploy to Heroku" button

<a href="https://www.heroku.com/deploy/?template=https://github.com/abraham-yusuf/web3-api">
<img src="https://assets.strapi.io/uploads/Deploy_button_heroku_b1043fc67d.png" />
</a>

2. Fill the Cloudinary ENV variables.
3. Deploy
4. Once is deployed, go to the admin panel e.g. `https://yourherokudomain.com/admin` and create an account.
5. Last, go to "Setting" > "Users & permissions plugins" > "Public" > "Permissions" and check `find` on Article, Category, Contributor and Pages.

### Adding Content

The recommended flow for adding new content is:

- Add contributor
- Add category
- Add article or page

### Preview Content

Once you have your frontend deployed go to "Settings" > "Preview Content"

Fill it with your info, the URL should look like this.
`https://<yoursite.com>/api/:contentType-preview?secret=<your-secret>&id=:id`

Now, go to any article or page and click on "Preview".

*Note: Preview Content is Optional*
