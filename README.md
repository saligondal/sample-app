# Sample App – CI/CD Pipeline Lab

Deze repository bevat een sample Flask applicatie voor een CI/CD-lab met Docker en Jenkins (DevNet Associate).

Doel van het lab:
- Code pushen naar GitHub
- Jenkins gebruiken om builds te starten
- Applicatie containerizen met Docker
- CI/CD pipeline opzetten en testen

Inhoud:
- sample_app.py – Flask webapplicatie
- templates – HTML templates
- static – Static bestanden
- sample-app.sh – Bash script voor Docker build en run
- tempdir/Dockerfile – Dockerfile (gegenereerd via script)
- run_docker_jenkins.sh – Script om Jenkins in Docker te starten

Flask applicatie runnen met Docker:
1. Script uitvoerbaar maken:
chmod +x sample-app.sh

2. Docker image bouwen en container starten:
./sample-app.sh

3. Controleren of de container draait:
docker ps

4. Applicatie testen:
Open http://localhost:5000 in de browser

Jenkins runnen met Docker:
1. Jenkins script uitvoeren:
chmod +x run_docker_jenkins.sh
./run_docker_jenkins.sh

2. Jenkins openen:
http://localhost:8080

Containers beheren:
- Draaiende containers bekijken:
docker ps

- Alle containers bekijken:
docker ps -a

- Container stoppen:
docker stop <container_naam>

- Container stoppen en verwijderen:
docker rm -f <container_naam>

Context:
Lab gebaseerd op “Build a CI/CD Pipeline Using Jenkins” (Cisco DevNet Associate).
