Please Install docker desktop before cloning this repo.
The installation comes with a fairly intuitive GUI to view and manage containers.

To clone run the following comands: 
git clone https://github.com/YOUR_USERNAME/Clinicia_ai_health.git
cd Clinicia_ai_health
docker compose up -d 

docker compose up -d boots up openwebui, might take quite some time the first time it is executed.

Run the following line to view status of the page. This also gives you more details about the cointaner such as its name. The website won't be ready until the status returns: (Health: Healthy)

docker ps

You may access the site through the following port
http://localhost:3000

Once you are ready to pull from branches after hcanges have been made, make sure to execute both of these lines so that both your local branch and container stay in sync:
git pull
docker compose restart

To terminate session:
docker stop NAME_OF_CONTAINER 
