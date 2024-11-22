
# Running the notebooks

## Registering an account

The NWFP APIs require you to register an account. You can do this via the registerUser API following these instructions or on our [NWFP Swagger page](https://api-nwfp.rothamsted.ac.uk).

To register a new user, follow these steps:

1. API Endpoint: api/auth/v1/registerUser/
2. Method: POST
3. Parameters:
   - email: Your email address
   - password: Your chosen password
4. Upon successful registration, you will receive a confirmation email. Please follow the instructions in the
email to confirm your registration.

## Logging in 

Once registered, you can log in using the following steps:

1. API Endpoint: api/auth/v1/login/
2. Method: POST
3. Parameters:
   - email: Your registered email address
   - password: Your password
4. Upon successful login, you will receive two tokens: an access token and a refresh token. Use the access
token for authentication in subsequent API requests.

The [NWFP_API_demo_login.ipynb](https://github.com/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_demo_login.ipynb) demonstrates python code for logging in and obtaining a bearer token.

## Using a .env file for your login credentials
Once registered you will need to login to the API in order to access the data. We recommend keeping your login credentials in a local .env file with the following properties:
- API_EMAIL
- API_PASSWORD

You may need to install the python-dotenv library. Do this with: 
```
!pip install python-dotenv
```

If you are using Google Colab to run the notebooks this would be located in your mounted google drive.

To mount your Google Drive in Google Colab run:
```
from google.colab import drive
drive.mount('/content/drive')
```

## How to Use Google Colab with GitHub

You can use Google Colab with GitHub to run the Jupyter samples included here. Follow these steps:

1. **Open Google Colab**:
   - Go to Google Colab.

2. **Open a Notebook**:
   - Select the **File** tab.
   - Click on **Open notebook**.

3. **Access GitHub**:
   - Select the **GitHub** tab on the left.
   - Enter the URL of the GitHub repository or the specific notebook you want to open.

4. **Choose and Open the Notebook**:
   - Choose the notebook from the list.
   - Click **Open**.

This operation will download the selected file from GitHub to your notebook. Now you can try this sample.

# The notebook examples

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg 'Open in Colab')](https://colab.research.google.com/github/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_demo_login.ipynb) 
**[NWFP_API_demo_login](https://github.com/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_demo_login.ipynb)** demonstrates logging in and obtaining a bearer token

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg 'Open in Colab')](https://colab.research.google.com/github/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_demo_farmlet_map.ipynb) 
**[NWFP_API_demo_farmlet_map](https://github.com/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_demo_farmlet_map.ipynb)** demonstrates using the getCatchments endpoint to retrieve and map catchment boundaries and view basic information

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg 'Open in Colab')](https://colab.research.google.com/github/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_demo_farmlet_map.ipynb) 
**[NWFP_API_demo_measurements](https://github.com/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_demo_meaurements.ipynb)** demonstrates using the getMeasurementsByTypeID. The example uses help features to explore data categories then retrieves different measurements using filters and plots the resulting data. 

<a target="_blank" href="https://colab.research.google.com/github/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_demo.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a><a href="https://github.com/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_demo.ipynb">NWFP_API_demo demonstrates fetching some data filtered by the API paramters</a>
<br>
<a target="_blank" href="https://colab.research.google.com/github/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_error_handling.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a><a href="https://github.com/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_error_handling.ipynb">NWFP_API_error_handling demonstrates demonstrates error handling</a>
<br>

<a target="_blank" href="https://colab.research.google.com/github/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/Catchments boundary map Demo.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a><a href="https://github.com/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/Catchments boundary map Demo.ipynb">NWFP_API_demo_farmlet_map demonstrates using the getCatchments endpoint to retrieve and map catchment boundaries</a>
<br>
<a target="_blank" href="https://colab.research.google.com/github/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/ChartsSample.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a><a href="https://github.com/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/ChartsSample.ipynb">ChartsSample.ipynb demonstrates using the requested data to draw some charts </a>




**[NWFP_API_demo_farmlet_map](https://github.com/North-Wyke-Farm-Platform/NWFP-API-Demo/blob/main/NWFP_API_demo_farmlet_map.ipynb)** demonstrates using the getCatchments endpoint to retrieve and map catchment boundaries