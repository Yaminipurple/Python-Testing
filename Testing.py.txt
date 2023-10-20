import requests


base_url = "http://127.0.0.1:5000"  


response = requests.get(base_url + "/")


if response.status_code == 200:

    print("Test Passed. Response:")
    print(response.text)
else:

    print(f"Test Failed. Status Code: {response.status_code}")
