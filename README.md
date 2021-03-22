# Streamlit_app_with_docker
Deploy Streamlit Apps with Docker

### Create a virtual env
python3 -m venv streamlitapp


### Activate the Virtual env
.\streamlitapp\Scripts\activate

### Install Streamlit in the env 
### Create a requirement file from this env 
pip freeze > requirements.txt

### Building the Image

docker build -t  <imagename:tagname>  .
eg : docker build -t  myapp:latest  .

### Check 
docker images 

### RUNNING THE IMAGE
docker run -p 8501:8501 myapp:latest
This port and the one in the docker file: Expose should be same 
Check the URLS or check localhost8501
