# API NOTES

## API README

Task-0

This fetches data from the specified API and prints the employee's TODO list progress in the specified format.

To use the script, save it to a .py file and run it from the command line, passing the employee ID as an argument. For example:

bash
python script_name.py 1

This will display the TODO list progress for the employee with ID 1. The script will use the requests module to interact with the API and retrieve the necessary information. The completed tasks will be printed with 1 tabulation and 1 space before the task title, just as specified in the requirements.

Task-1

This provided script is exporting data in CSV format for a given user ID using the jsonplaceholder API. It gathers user-specific data and tasks from the API and writes the information to a CSV file.

Here's a summary of what the script does:

It imports the necessary modules, csv and requests.
It defines a get_api() function to gather data from the API based on the provided user ID.
Inside the function, it uses requests.get() to retrieve the user's data and task information using the given user ID.
It opens a CSV file in write mode using the provided user ID as the filename, and it writes the data into the CSV file using the csv.writer().
The CSV file will contain the following columns: user_id, username, completed, and title.
The script is designed to be executed from the command line, where the user ID is passed as an argument (argv[1]).
To use the script, save it to a .py file and run it from the command line, passing the user ID as an argument. 

This will create a CSV file named 1.csv containing the user-specific task information for the user with ID 1.

The script is a simple and effective way to export data from the API to a CSV file based on the provided user ID.

Task-2


This script exports data in JSON format for a given user ID using the jsonplaceholder API. It gathers user-specific data and tasks from the API and writes the information to a JSON file.

Here's a summary of what the script does:

It imports the necessary modules, json and requests.
It defines a get_api() function to gather data from the API based on the provided user ID.
Inside the function, it uses requests.get() to retrieve the user's data and task information using the given user ID.
It opens a JSON file in write mode using the provided user ID as the filename, and it constructs a JSON object to store the data.
The JSON object is a dictionary where the user ID is the key and the value is a list of dictionaries containing task information, including task, completed, and username.
The script is designed to be executed from the command line, where the user ID is passed as an argument (argv[1]).
To use the script, save it to a .py file and run it from the command line, passing the user ID as an argument. For example:

This will create a JSON file named 1.json containing the user-specific task information for the user with ID 1.

The script is an effective way to export data from the API to a JSON file based on the provided user ID. It uses the json.dump() method to serialize the Python object into a JSON stream, ensuring that the data is stored in a valid JSON format.

Task-3

This provided script is another version of the script to export data in JSON format, but with a slight modification. It now exports the TODO list data for all employees instead of just one employee.

Here's a summary of what the updated script does:

It imports the necessary modules, json and requests, and gives an alias r to the requests module for brevity.
It defines a get_api() function to gather data from the API for all employees.
Inside the function, it uses r.get() to retrieve all users' data and tasks from the API.
It iterates through each user and creates a dictionary with the user ID as the key and a list of dictionaries containing task information as the value.
Each task dictionary contains username, task, and completed information for that specific user.
The script then writes the data to a JSON file named todo_all_employees.json.
To use the script, save it to a .py file and run it. The script will fetch data for all employees and store it in a JSON file as described above.

This updated version is useful if you want to export the TODO list data for all employees into a single JSON file for further analysis or processing.
