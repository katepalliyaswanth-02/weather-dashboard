# weather-dashboard
1.
#Configure AWS
  aws configure
Enter Access Key, Secret Key, Region, Output format.

2.#Get API Key
#Sign up at OpenWeatherMap
#create and sign in openweathermap
#Access key id and secret access key

3.#Set Environment Variables
Create a .env file:
PENWEATHER_API_KEY=
AWS_BUCKET_NAME=

4.# Install Dependencies
pip install -r requirements.txt

5.#Run Script
python weather_to_s3.py
First run → Creates bucket + uploads weather JSON.
Next runs → Reuses bucket + uploads new JSON with timestamp.

6.#Validate
Check bucket in AWS Console.
Or list files:
aws s3 ls s3://<your-bucket-name> --recursive
Download and open a file to confirm valid weather JSON.
