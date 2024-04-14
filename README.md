# Explain-this-to-me
App to help simplify key idea and concepts to help students in their writing process
## Table of Contents
- [What is contained with in] (#whats-contained)
- [How to Use] (#How to use)
- [Installation](#installation)
- [Usage](#usage)
- [Problems](#Problems)
- [License](#license)

## What is contained with in
A list of some of the more important files found in the app:
1. requirements.txt; A text file that lists and shows all the requirements sothat the app can run properly.
2. init_db.py; the first file that must be run before anything else because its job is to it initializes the database
3. Schema.sql; this file as the name implies provides SQL code that is used to handle the information that is inputted during the apps use. By doing so the app can properly provide feedback to users regarding their consent forms, and insuring that it is doing its job properly 
4. database.db; this file stores the data inputted into the application as given by the instructions given by the before mention schema.SQL file
5. app.py; this is the app itself in its current form. It is very important because it is what will be run in your temrinal throughout this process.
## How to use
The app is configured to run with Flask. If you have Python and Flask, you can clone this repository and run it using `flask run`.
The app takes user input and runs the result using OpenAI's Chat API. The system is configured using the following query:
> Students will provide a complex idea or concept that they are having trouble understanding
>   The chatbot will then explain whatever concept or idea that have asked about in terms that are simple to understand and as if they are only 12 years old
## Installation
For proper installation a user must first 
1. Install PYTHON 3,  This can be done by going to the python website and following the steps listed for your type of computer, the recent and up to date python releases can be found here: https://www.python.org/downloads/ I would recommend installing the latest release to make sure you have the easiest time while installing/running everything needed for this app. IF YOU ALREADY HAVE PYTHON 3 INSTALLED SKIP TO NEXT STEP
2. Install PIP, you should get pip pre-installed when downloading from python.org, but still it is a good idea to check your own machine and if not found it must be installed for the rest of the needed elements to be properly installed. If you find that you do not have it installed those who are  maintainers for pip have provided commands to install and upgrade it for for Windows, MacOS, and Linux here: https://pip.pypa.io/en/stable/installation/. IF YOU ALREADY HAVE PIP INSTALLED SKIP TO NEXT STEP
[NOTE FOR NEXT STEPS: For further instructions please go to https://platform.openai.com/docs/quickstart?context=python]
3. Install FLASK, to do so you must open your terminal and input:
pip install flask. 
4. Install OPENAI, still with in your terminal You can install OpenAI's python library by inputting: 
pip install --upgrade openai 
5. You then need to further configure OpenAI bby usinng your unique OpenAI API key, this is provided by creating an account with OpenAI and then ensuring it is attached to your computer. The Link above will provide the steps that needs to be followed for the diffrent types of systems that is being used.
## Usage
Now that you have everything installed you can start using your app. Hooray!
1. Now that you have flask and OpenAI's python library installed it is time for the next step. Now you need to initialize the db file before you can run the app. You can do this by inputting this in to your terminal: 
python3 init_db.py (If that does not work input instead python init_db.py)
2. It is now show time! You can now run your app and to do so in your terminal input: 
python3 -m flask --app app run
3. You should have gotten from flask a link for the local host address, go to it and this should bring you to a webpage where you can expriment with the app to see how it runs and decided if there are any changes you wish to be made.
## Problems
- OpenAI is a bit slow as of date of instalation 2024-04-14
## License
This project is licensed under the [MIT License] (LICENSE) 
