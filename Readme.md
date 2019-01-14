# Magento Backend Developer Challenge

As a Magento Backend developer, we need more than making code to create functionality. So this test is going to be split into several sections with a different kind of challenge.

If you have any issue understanding some concepts you can find more information here [PHP The Right Way](https://phptherightway.com/)


## First Challenge

We are going to use Docker for use Nginx/Apache, PHP 7.1.13, MySql, so the first step is to create a new project with Magento and serve new Website using Docker together with MySQL, the PHP version need to be the highest for Magento 2. After you finish with the configuration is expected to have a port on your machine running a web server through Docker. In this step, we need to do all the Magento configuration and serve a proper website showing dummy products. 

####Considerations
- Create a database
- Use docker compose for handling docker configuration
- You can use the existent configuration on the internet to achieve this step
- MySql, Apache or Nginx need to run in a docker container 
- One line script is required to spin up the project, preferable ```docker-compose up -d```


## Second Challenge

Now that we have a dummy website using Magento is time for do some real work. 

Install and use the Cloudinary Plugin, you can create a free account [here](https://cloudinary.com/)

**All images** should be served from cloudinary.

## Third Challenge

Create a [Service Worker](https://developers.google.com/web/fundamentals/primers/service-workers/) and add all the static images, no products images, in the static cache. The Service Worker should show up in every URL. 


## Forth Challenge

Create a new Module for the Product Page to add to the service worker the main image of the product, not all, just the main one. This image needs to be cached being added to the service worker. 

#####Considerations
- The static images from the previous challenge should be kept there, so you only need to add new ones. 
- Avoid duplications
- You can save up to 10 product images in the cache, after that you need to fill the new ones replacing the oldest


## Fifth Challenge

Test all the things. We are going to focus on behaviour tests, no need for unit test but will be a plus if is properly implemented and separated from the behaviour Test.

We are going to test the happy path for conversion. 

- Be able to go to the homepage and do a search
- Get a Product in a listing, clicking in the 3rd one
- Add the product to the cart
- Go through the checkout process until the payment is required. 


## Lately 

Document the project, how to spin up the project, how to run the tests and how to generate the database and the dummy content. This will be preferable to have it in only one bash scripts but you will decide. 

After you have the documentation, create a repository in GitLab/Github/Bitbucket and send us the link of the repository to {{Chalhoub Email}}


We are going to give you feedback as fast as possible. 

