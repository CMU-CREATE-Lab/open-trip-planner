# open-trip-planner

Python code for generating summaries of census block centroid transit routes for the City of Pittsburgh and Allegheny County.

# Installation
$ cd open-trip-planner
$ python -m venv venv
$ source venv/bin/activate
$ pip install -r requirements.txt 

## Run OpenTripPlanner 
$ java -Xmx10G -jar otp-1.5.0-shaded.jar --basePath otp --build otp --inMemory 
## Run OpenTripPlanner as a background process on a non standard port
$ nohup java -Xmx10G -jar otp-1.5.0-shaded.jar --basePath otp --build otp --inMemory --port 9090 --securePort 9091 & 

## Run a notebook as a background process on a non standard port
$  nohup jupyter notebook --port=9941 --port-retries=0 &
