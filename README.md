# Een Flask applicatie in een container


```bash
# Builde the image
docker build -t flask-tutorial:1 .

# docker run 
# -rm: verwijder als gestopt
# -d: in de achtergrond
# --name: met de naam flask-tutorial-app
# -p 5000:5000: verbind de extrene poort 5000 met de poort 5000 in de container
# flask-tutorial: gebruik deze image
docker run --rm -d --name flask-tutorial-app -p 5000:5000 flask-tutorial:1


# Bekijk de logs
#-f: volg de logs
docker logs -f flask-tutorial-app
```
