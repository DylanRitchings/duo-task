# Use Python 3.6 or later as a base image
FROM python:3.6

# Install apt dependencies
RUN apt update && apt install -y python3-pip 

# Copy contents into image
COPY . .
# Install pip dependencies from requirements
RUN pip3 install --upgrade pip && pip3 install flask && pip3 install flask-sqlalchemy && pip3 install pymysql 
# Set YOUR_NAME environment variable
ENV YOUR_NAME="AADIL"
# Expose the correct port
EXPOSE 5500
# Create an entrypoint
ENTRYPOINT ["/usr/local/bin/python", "app.py"]