# Agile-Assignment-1

Name of webApp: Agree or Disagree

Created by: Barry Cronin Student Num: 20074828 
github link to project: https://github.com/bazcron/Agile-Assignment-1

This is my API test automation & Source Control Project.

Using my original webApp code for AgreeORdisagree i implemented tests for the 2 models i currently have,
Statements and Users.

Statements Model:
let mongoose = require('mongoose');
let statementSchema = new mongoose.Schema({
        id: Number,
        statement: String,
        agree: Number,
        disagree:Number
    },
    { collection: 'statements' });
module.exports = mongoose.model('statements', statementSchema);

Users Model:
let mongoose = require('mongoose');
let usersSchema = new mongoose.Schema({
        id: Number,
        name: String,
        email: String,
        password: String,
        agree: Number,
        disagree: Number
    },
    { collection: 'users' });
module.exports = mongoose.model('users', usersSchema);


I opened a terminal and set up an initial git repository inside the project folder: git init

i then created a .gitignore file with the following text: 
/node_modules
*.log
package-lock.json
/**/.DS_Store*
*DS_Store*

which excludes all the node_modules, log files and anything named .ds_store

i set up an initial commit:
git add -A 
git commit -m "Initial project structure"

i then ran: npm install

i then ran:
git checkout master, to make sure it was on the master branch
i then created a new branch: git branch add-users-test

where i added my test code to the project and ran the tests, all tests passed

i then went back to the master branch, git checkout master
i then merged the branch with git merge add-users-test

i then created another branch, add-statements-test
and wrote and tested test code for the statement route

this was also merged and pushed to github.


References: https://moodle.wit.ie/course/view.php?id=163135&section=7
