# Use Python 3.6 or later as a base image
FROM python:3.6
# Copy contents into image
COPY . .
# Install pip dependencies from requirements
RUN pip install Flask
# Set YOUR_NAME environment variable
ENV YOUR_NAME="Haydon"
# Expose the correct port
EXPOSE 5500
# Create an entrypoint
ENTRYPOINT ["/usr/local/bin/python3", "app.py"]
