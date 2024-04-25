# MarketPeak_Ecommerce Website

# How I approached the Challenge:

# Creating my git repository and initialization:

1. I created my git repository called MarketPeak_Ecommerce and initialized.
2. I downloaded the website files from the link provided in the capstone project, staged to the repo, commit it and push to my git repository (main branch).

# Creating an EC2 Instance on AWS and setting it up:

1. I created an ec2 instance on aws using the free tier amazon linux.
2. Updated it using the: sudo yum update -y
3. Cleared the /var/www/html/ directory by removing all the files
4. Cloned my git repository using the (https option) in the /var/www/html/ directory
5. Installing the apache server using: sudo yum install httpd -y
6. Started the Apache web server using : sudo systemctl start httpd
7. Reloaded the server to include new changes using: sudo systemctl reload httpd

# With the httpd configured:

1. With httpd configured and website files in place, MarketPeak Ecommerce platform is now live on the internet:
2. I open a web browser and accessed the public IP of my EC2 instance to view the deployed website.

# Performed Continuous Integration & Continuous Deployment:

1. I went back to my web files
2. Created a new branch, called "development" using: git checkout -b development
3. I made a change in the index.html file
4. Add my changes using: git add .
5. Committed my changes using: git commit -m "change details"
6. Pushed my changes to the origin development branch: git push -u origin development
7. Went to my github page, created a PR and Merged the changes to my main branch
8. On my editor, switched to my main branch and merged the changes from the development branch: git merge development

# Updating the Changes on EC2:

1. Went back to my /var/www/html/ folder and created a git pull to invoke the latest changes
2. I reloaded my apache server to reflect the changes on my web site: sudo systemctl reload httpd

PS: The process was quite straigthforward and I didn't encounter any challenges. It was a wonderful experience to practicalize the teaching and understand how it works in real life scenario.
