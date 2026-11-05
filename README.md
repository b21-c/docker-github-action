This project uses Docker and GitHub Actions to automate deploying a static foosball website. 
Docker packages the site’s HTML pages and web server into a portable image, defined by the Dockerfile in the foosball folder, so the app runs the same way on any machine with a single command. 
A GitHub Actions workflow (.github/workflows/docker.yml) runs on every push to the repository: it checks out the code, 
logs in to Docker Hub using credentials stored as GitHub secrets, builds the image, and pushes it to Docker Hub tagged with the workflow run number 
