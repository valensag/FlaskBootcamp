# Introduction
## Create a virtual env with Conda
```
conda create -n flaskenv
```
## Activate virtual env
```
source activate flaskenv
```
## Install a new version of Python
```
conda install python=3.9
```
## Instll requirements.txt
```
pip install -r requirements.txt
```

# What can I do with Flask
- Accept info from user
- Retrieve information from a database
- Create/ Update/Delete information in a database
- Display info back to the user

To permorm these task, we'll need a web framework to accept and return information with the front end.

To collect the info of the user we will use a library called <ins>WTForms</ins> 

To communicate with the database and retrive information we will use <ins>SQLAlchemy</ins> and to update the info in the database <ins>Flask-Migrate</ins>

To return the info to the user, we will use <ins>Jinja Template</ins> that grab info from python and flask to send info back as HTML

> Flask renders **HTML** templates, can edit them with **Jinja** and can communicate with a database using libraries such as **SQLAlchemy**

# Forms
- To connect a label with a input box use the id
```
<form action="http://www.google.com" method="GET">
    <label for="emailtag">Email:</label>
    <input id = "emailtag" type="email" name="useremail" placeholder="Email Here">
    <br>
    <br>
    <label for="passtag">Password:</label>
    <input id = "passtag" type="password" name="userpassword" placeholder="Password">
    <br>
    <br>
    <input type="submit" value="submit">
</form>
```

- Link Radio Button
- Drop down Menu
- Text area inputs

```
<form method="get">
        <h3>Do you already own a dog?</h3>
        <label for="yes">Yes:</label>
        <input type="radio" id = "yes" name="dog_choice" value="yes">
        <label for="no">No:</label>
        <input type="radio" id = "no" name="dog_choice" value="no">

        <p>How clean is your house= (1-3)</p>
        <select name="stars" id="">
            <option value="Great">3</option>
            <option value="Good">2</option>
            <option value="Bad">1</option>
        </select>

        <p>Any other comments?</p>
        <textarea name="name" id="" cols="80" rows="8"></textarea>
        <br>
        <input type="submit" value="Submit Feedback">
```


 