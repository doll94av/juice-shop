# Outline of setting up Juice Shop

- Fork Juice shop to my personal github account: https://github.com/doll94av/juice-shop

- Clone the repository to a local machine (PI): gh repo clone doll94av/juice-shop

- Install prequisites via apt-get for NPM and NVM for managing the node version

- Update NodeJS to a version that is in the supported range for Juice-Shop

- NPM install to install deps

- NPM run to deploy the application

- Deploy application and make it publically available: http://69.14.248.76:3000/#/


## Merge and best practices

- Merging to main can be dangerous. When code changes you may end up implementing a breaking change which causes the app to crash and teams to have to firefight instead of focusing on developing. Code should always be merged to a feature branch / development branch, tested, then merged to main when it is ready to go to production.

- Preventing this is best done by implementing good CI processes for testing but also configuring your SCM to not allow merging to main along with configuring branch protection rules that rely on tests passing to merge code