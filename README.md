# korona Dashboard

## Development

Clone the repo and install `node_modules` using `yarn` or `npm install`.

Start development with `npm run dev` command which should open the site in your browser `http://localhost:3000`.

## CI CD

I uses CircleCI as a CI CD service.


The CI implemetion exist in .circleci/config.yml file.

This pipline will trigger for each commit.

## The pipline do the below actions:
1. Build new docker image with the last changes
2. Push the new image to dudi938/korona_dashboard repo on docker hub
3. deploy via ssh the new image to the ec2 instance
   note: if the korona_dashboard already on on the ec2 vm then i kill him and run the new image.


## More info

The app running on ec2 instance and available in url http://3.21.190.19:3000



